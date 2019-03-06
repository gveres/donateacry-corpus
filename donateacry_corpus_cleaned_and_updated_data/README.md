# donateacry-corpus-cleaned-updated
<p>An infant cry audio corpus based on https://github.com/gveres/donateacry-corpus</p>
<p>This updated corpus is used as part of final project in Speech Technology Course in KTH (Royal Institute of Technology Sweden)</p>
<p>Our group members are: Arra’di Nur Rizal - Jonathan Jan - Luise Dürlich - Shifei Chen</p>

## Source of these files
This folder contains cleaned and categorized data from https://github.com/gveres/donateacry-corpus

## Updates to the original
- All of the data have been converted to WAV format with uniform bit and sampling rate of 128 kbps and 8kHz
- Using DBL (Dunstan Baby Language) categories as reference, data tagged with lonely, scared, and unknown are removed. Additionally data tagged with cold/hot was merged into discomfort.
- All non-cries data has been removed manually by listening to them. These includes, white noise, baby chat, adult mimicking baby cries. etc.
- All data are put into its respected folder without changing the original filename.

## File naming convention
The audio files should contain baby cry samples, with the corresponding tagging information encoded in the filenames. The samples were tagged by the contributors themselves. So here's how to parse the filenames.

```
iOS:
0D1AD73E-4C5E-45F3-85C4-9A3CB71E8856-1430742197-1.0-m-04-hu.caf
app instance uuid (36 chars)-unix epoch timestamp-app version-gender-age-reason
```
So, the above translates to:
- the sample was recorded with the app instance having the unique id 0D1AD73E-4C5E-45F3-85C4-9A3CB71E8856. These ids are generated upon installation, so they identify an installed instance, not a device or a user
- the recording was made at 1430742197 (unix time epoch) , which translates to Mon, 04 May 2015 12:23:17 GMT
- version 1.0 of the mobile app was used
- the user tagged the recording to be of a boy
- the baby is 0-4 weeks old according to the user
- the suspected reason of the cry is hunger

```
Android:
0c8f14a9-6999-485b-97a2-913c1cbf099c-1431028888092-1.7-m-26-sc.3gp
The structure is the same with the exception that the unix epoch timestamp is in milliseconds
```

## Tags
### Gender
- *m* - male
- *f* - female

### Age
- *04* - 0 to 4 weeks old
- *48* - 4 to 8 weeks old
- *26* - 2 to 6 months old
- *72* - 7 month to 2 years old
- *22* - more than 2 years old

### Reason
- *hu* - hungry
- *bu* - needs burping
- *bp* - belly pain
- *dc* - discomfort
- *ti* - tired

## License
*This donateacry-corpus is made available under the Open Database License: http://opendatacommons.org/licenses/odbl/1.0/. Any rights in individual contents of the database are licensed under the Database Contents License: http://opendatacommons.org/licenses/dbcl/1.0/ - See more at: http://opendatacommons.org/licenses/odbl/#sthash.ejQJkkvi.dpuf*
