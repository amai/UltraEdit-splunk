# UltraEdit wordfile (.uew) for Splunk

A quick effort cobbling together a [wordfile for UltraEdit](http://wiki.ultraedit.com/Wordfiles) to pretty-up [Splunk .conf files](http://docs.splunk.com/Documentation/Splunk/7.1.0/Admin/Listofconfigurationfiles).

Generally adequate support for the following, so far:
* app.conf
* fields.conf
* indexes.conf
* inputs.conf
* outputs.conf
* props.conf

At the top level, stanzas have been defined, broadly, where square brackets are at the start of a line and everything contained within them becomes the stanza name. The stanza names, as defined, populate themselves under the *Function List* on UltraEdit for quick and useful jump-to points.

**Issues/TODO:**
* The color keywords section is a mess.
  * Reorganize hierarchy of keywords
  * Sort case-sensitive values better
  * Substrings handling is incomplete/inconsistent
* Add highlighting for search commands (see [`savedsearches.conf`](http://docs.splunk.com/Documentation/Splunk/7.0.3/Admin/Savedsearchesconf))
* Parse and tier stanzas by type
* Include handling for remaining [.conf files](http://docs.splunk.com/Documentation/Splunk/7.1.0/Admin/Listofconfigurationfiles)
