DIY Transcription Site
=====================

DIYHistory is built upon the open-source generosity of George Mason University's [Center for History and New Media](http://chnm.gmu.edu/), so we feel it's only right to give our sourcecode out to organizations and individuals interested in implementing their own crowdsourcing initiatives. Anyone who can install Omeka and MediaWiki on a web server can easily get started with their own branded version of DIYHistory|transcribe with little to no programmer time. If you find our code useful and build further upon it, we'd love to receive your pull requests at [github.com/ui-libraries](https://github.com/ui-libraries).

##Overview
[DIYHistory|transcribe](http://diyhistory.lib.uiowa.edu/transcribe) is a tool for engaging users in transcribing handwritten documents, making them more searchable and enhancing them for research. [DIYHistory|transcribe](http://diyhistory.lib.uiowa.edu/transcribe) is built on the [Omeka](http://omeka.org/) content management system and uses the [Scripto](http://scripto.org/) plugin to facilitate transcription. [Scripto](http://scripto.org/) uses [MediaWiki](http://www.mediawiki.org/wiki/MediaWiki), which allows users to continually improve upon work that has already been done. In building this site, we made significant additions to the Scripto plugin, created a new Omeka theme, and customized other Omeka plugins to style and scale for a library production environment.

##Requirements
[DIYHistory|transcribe](http://diyhistory.lib.uiowa.edu/transcribe) requires the following:

- [Omeka version 2.x](http://omeka.org/codex/Version_History)
- [Omeka Dublin Core Extended plugin] (http://omeka.org/add-ons/plugins/dublin-core-extended/)
- [Daniel-KM/CsvImport](https://github.com/Daniel-KM/CsvImport), a fork of Omeka’s CsvImport that allows bulk upload of item and file-level metadata
- [ui-libraries/plugin-Scripto](https://github.com/ui-libraries/plugin-Scripto), a fork of CHNM’s Scripto tool for crowdsourced transcription of documents. Scripto requires a [MediaWiki](http://www.mediawiki.org/wiki/MediaWiki) installation.
- [Scribe](https://github.com/ui-libraries/Scribe), a custom Omeka theme designed for use with ui-libraries/plugin-Scripto

##Features
[DIYHistory|transcribe](http://diyhistory.lib.uiowa.edu/transcribe) introduces the following features to plugin-Scripto:

- Track completion status of document pages (i.e., ‘Not Started’, ‘Needs Review’, ‘Completed’)
- Track completion progress of documents based on page statuses.
- Sort documents within their collection by most completed, floating least completed to the top.
- Initialize document page text entry box with pre-existing text, if available (helpful if using Scripto to correct OCR for typescript pages).
- On every page action, automatically import transcriptions from MediaWiki as file metadata.


The [Scribe](https://github.com/ui-libraries/Scribe) theme directs its focus on guiding users to easy transcription tasks rather than collection management features, offering a clean, thumbnail-oriented transcription view for any number of Omeka image collections.

By default, any member of the public is allowed to edit and save transcription data, but only users with an account can track their progress. Approved account holders can also be granted administrator (or deputy) status, allowing them to finalize documents as “complete”.

## Installation
Follow the documentation at each source code repository to install [Omeka 2](http://omeka.org/codex/Version_History), [ui-libraries/plugin-CsvImport](https://github.com/ui-libraries/plugin-CsvImport), [ui-libraries/plugin-Scripto](https://github.com/ui-libraries/plugin-Scripto) + [MediaWiki](http://www.mediawiki.org/wiki/MediaWiki), and [Scribe](https://github.com/ui-libraries/Scribe). 
