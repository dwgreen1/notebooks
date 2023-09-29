# To Create a New List
`sudo /usr/lib/mailman/bin/newlist list@example.com`


# Email Forwarding
Must be done for regular OPAL emails that need to be forwarded to ohionet.org

  * Edit: `/etc/postfix/main.cf`
  * Restart: `sudo /etc/init.d/postfix reload`


# Push Options to a List
`./config_list -i global_options.txt listname`


# Remove Member from All Lists
`sudo /usr/lib/mailman/bin/remove_members --fromall user@example.com`
