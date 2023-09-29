# Cheatsheet

## AWS File Path
https://library.ohio.gov/static/lsta/Instructional-Survey-for-Public.docx

## Font Awesome

Right Caret
```html
<i class="fa fa-solid fa-angle-right">&nbsp;</i>
```

## Grant Template
```html
<blockquote dir="ltr">
<p dir="ltr">Guiding Ohio Online application period has ended. The following is provided for information purposes only.</p>
</blockquote>

<h2 dir="ltr">About</h2>

<h2 dir="ltr">Request for Proposals</h2>

<h2 dir="ltr">Apply</h2>

<p dir="ltr">The Guiding Ohio Online application period has ended.</p>

<h2 dir="ltr">Final Narrative Report</h2>

<p dir="ltr">The Guiding Ohio Online reporting period has ended.</p>

<h2 dir="ltr">Final Financial Report</h2>

<p dir="ltr">The Guiding Ohio Online reporting period has ended.</p>

```

## Filter Resource Settings
```html
<script>
var IOPFilter = {};
//IOPFilter.menuComponent = '[Component name="ohio design/site-builder/site-components-core/filter/resources/menu-iop-resources-in-current-location-by-publish-date-desc" format="id"]';
IOPFilter.showKeyword = true;
IOPFilter.showDropdown = false;
IOPFilter. showDatePicker = false;
//IOPFilter.elementsPerPage = 8;
//IOPFilter.imageNoResults = '[Component name="ohio design/site-builder/odx-default-images/no-results.png" rendition="auto" format="url"]';
</script>
```

## Portal Location for Featured Resources
**Portal Location**
Select portal locations where you want to promote this item. Add Categories  
Taxonomy / Portal Locations / All Portal Locations / Common Locations / IOP Site Components / Popular Topic X  
Taxonomy / Portal Locations / All Portal Locations / By Agency / LIB / For Libraries  


## How I set up Databases Filter Catalog:
**Single Database**  
/Taxonomy/Portal Locations/All Portal Locations/By Agency/LIB/For Libraries/Databases  

**Databases Landing Page**  
/Taxonomy/Portal Locations/All Portal Locations/Common Locations/IOP Site Components/Landing Page Catalog  
/Taxonomy/Portal Locations/All Portal Locations/By Agency/LIB/For Libraries/Databases  

** The JS **
```javascript
<script>
var IOPFilter = {};
IOPFilter.menuComponent = '[Component name="ohio design/site-builder/site-components-core/filter/resources/menu-iop-content-matching-category-by-name-and-title-asc" format="id"]';
IOPFilter.category = '[Property context="current" type="content" field="categories" include="exact" format="namepath" restrict='taxonomy/lib']';
IOPFilter.showKeyword = false;
IOPFilter.elementsPerPage = 8;
IOPFilter.showDropdown = true;
IOPFilter.showDatePicker = false;
</script>
```
## Something try with Context?
```html
<!-- START: Ohio Design / Agencies / OCJS / Wrappers / WRAPPER - Home Latest News (5 Items) ->
[InContext context="selected" uuid="50af0d7a-262c-45c0-bcad-73a3f558fdd1"]]
[Component name="ohio design/site-builder/site-components-core/news/latest-news/main-latest-news" resultsPerPage="5" startPage=''*]
[/InContext]
<!-- END: Ohio Design / Agencies / OCJS / Wrappers / WRAPPER - Home Latest News (5 Items) >
```