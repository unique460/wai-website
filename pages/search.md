![46CA8F5C-5AFF-4784-AD76-B87B6EFB0904](https://github.com/user-attachments/assets/f2786f07-dfa8-427c-ac54-02dcbac9a0ca)
![B140D99B-EA89-47FF-933E-611693ABC928](https://github.com/user-attachments/assets/847bbd73-71d9-4e63-a9f5-c0bef6d62b13)


https://github.com/user-attachments/assets/49c797c6-fde5-47b9-b80a-3b664cca8033

---
title: Search
layout: default
permalink: /search/
tipue_search_active: true
exclude_from_search: true
---
<script src="{{ "/assets/scripts/jquery.min.js" | relative_url }}"></script>
<script src="{{ "/assets/search/tipuesearch_content.js" | relative_url }}"></script>
<script src="{{ "/assets/search/tipuesearch_set.js" | relative_url }}"></script>
<script src="{{ "/assets/search/tipuesearch.js" | relative_url }}"></script>

<strong>This page searches accessibility introductory and educational materials on the WAI website.</strong>

You can also:

* [Search W3C standards, guidelines, and Notes](https://duckduckgo.com/?q=site%3Aw3.org%2FTR&t=hf&ia=web), including accessibility and other areas
* [Search the entire W3C website](https://duckduckgo.com/?q=site%3Aw3.org&t=hf&ia=web)

## Search Form

<form action="{{ page.url | relative_url }}" class="searchform">
    <label for="tipue_search_input">Search:</label>
    <input type="search" name="q" id="tipue_search_input" pattern=".{3,}" title="At least 3 characters" required>
    <button class="button button--icon" type="submit">
     <span>{% include icon.html name="search"%}</span>&nbsp;<span>Search</span>
    </button>
</form>

## Search Results

<div id="tipue_search_content"></div>

<script>
$(document).ready(function() {
  $('#tipue_search_input').tipuesearch();
});
</script>

