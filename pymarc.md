PyMARC Examples
============

## Delete records matching criteria

<pre><code class="python">
from pymarc import MARCReader, Record, Field

FILE_IN  = ''
FILE_OUT = ''

with open(FILE_OUT, 'wb') as out:
	with open(FILE_IN, 'rb') as fh:
		reader = MARCReader(fh)
		for record in reader:
			if 'Springer' not in record['990']['b']:
				out.write(record.as_marc())
			else:
				print('Skipping: ' + str({record['990']['b']}))
</code></pre>

## Reorder fields in expected order

<pre><code class="python">
from pymarc import MARCReader, Record
​
FILE_IN  = ''
FILE_OUT = ''

with open(FILE_IN, 'rb') as fh, open(FILE_OUT, 'wb') as output:
    reader = MARCReader(fh)
    record_count = 0
    for record in reader:
        new_record = Record()
        # Reorder the fields into a new record object
        for field in record.get_fields():
            new_record.add_ordered_field(field)
        record_count += 1
        output.write(new_record.as_marc())
​
print(f'Records Processed: {record_count}')
</code></pre>
