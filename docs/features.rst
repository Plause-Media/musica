Features and Limitations
=================================

Key features and limitations of DMP are listed below. 
DMP works for most publishers world-wide, but not nearly for all.

By reading this section, you may save a lot of your time.

Remember, DMP is open-source, you are free to modify it to 
suit your needs. But this may require serious development.

If you need more than vanilla DMP, 
but don't have the knowledge or time or money to go into custom 
development, 
`That Green Thing <https://matijakolaric.com/thatgreenthing>`_, available as 
affordable Software-as-a-Service, is the recommended solution.

Music metadata management
-------------------------

The database can store detailed metadata for musical works and recordings, 
data about writers, recording and performing artists, releases (albums), 
labels and music libraries, as well as CWR exports and acknowledgements.

Total data validation
-------------------------

All entered data is validated for CWR and DDEX compatibility on field-, record-,
and transaction-level.

The flip side of the coin is that you can not enter incomplete data into 
DMP and hope to fix it later. The authors do not believe in fixing in post.

Single controlled publisher
-------------------------------------

DMP supports only a single controlled publisher (single publishing entity),
entered through settings. It will **not work** for publishers with multiple
entities, most notably US publishers affiliated with multiple PROs. 

Manuscript shares
------------------------

DMP uses a **single manuscript share** model, splits between writers 
(prior to publishing) are same for performance, mechanical and 
synchronisation rights.

Original publishing agreement data
-----------------------------------------

Basic **original publishing agreement** data can be entered, sufficient for 
registrations in societies that require **society-assigned agreement numbers**.

Share transfer
-------------------------

Share transfer from a controlled writer to the publisher can be configured, 
in accordance with national regulations and customs. There is only a **single 
setting for all controlled writers**.

Default is *London rule* (50% performance, 100% mechanical).

Publisher fees
-------------------------

Publisher fees are customisable per-writer, or even per-writer-per-work.

No other publishers
------------------------

It does **not** manage data for **other publishers**. Non-controlled writers 
appear as unpublished in CWR files. 

Co-publishing
------------------------

**Co-publishing deals** are possible, with each publisher registering their own 
shares. In this case, the other publisher appears as unknown in CWR files.

No support for composite works
--------------------------------

Composite musical works, as well as recordings based on multiple musical works 
(e.g. medleys), are not supported.

Registrations
-------------

Registrations can be exported as **CWR** files. Supported versions are: 2.1, 2.2, 3.0, 
and 3.1.

Acknowledgement files in CWR format can be imported.

**CWR preview** features syntax highlighting with additional data on mouse-over,
for both CWR files generated by DMP and imported acknowledgements.

Defaults when creating CWR files
---------------------------------------

When creating CWR, many fields are left with blank/zero values. When the fields are 
required in CWR, it uses reasonable defaults, e.g.:

* *Musical Work Distribution* is set to *Unclassified*,
* *Recorded indicator* is set to *Yes* or *Unknown*, depending if recording 
  metadatawas entered, and
* *Work for Hire*, *Grand Rights Indicator*, *Reversionary Indicator*, and *First 
  Recording Refusal Indicator* are set to No.

Royalty management
--------------------

**Incoming royalty statements** in CSV format can be processed, resulting in 
CSV statements containing data for distribution between controlled interested 
parties. Statement processing is extremely fast.

Actual outgoing statements must be created in Excel using pivot tables. For
experienced Excel user, this takes about 10 minutes for the first statement and
then about 30 seconds per statement for all others. 
This process can be fully automated by using scripts.

Data imports and exports
------------------------

Data about works can be imported from *CSV* files.

Data for selected works can be exported as *JSON* (complete) or *CSV* (partial).

Audio files and images
------------------------

If persistent file storage is available, images can be uploaded (photos for
writers and artists, logos for labels, cover arts for releases), as well as
audio files.

Sharable playlists
----------------------

Playlists can be created and shared, protected only by secret URLs.

REST API
----------------------

Read-only REST API, with basic HTTP authentication, is available. 
It can be used for:

* Complete data export
* Metadata exchange
* Content exchange
