# Dead by Daylight Resource Packs
This is the Packs Registry for the [DBD Resource Pack Manager](https://github.com/Charzard4261/DBD-ResourcePackManager). It is automatically checked on program start once every 12 hours, and can be mannually triggered in the settings.

## Submitting a Pack
To submit a pack, your pack should have the following file structure, and be uploaded to a site that allows for a direct download link (Google Drive, Dropbox, etc).
```
Pack.zip
  ├── Actions
  ├── CharPortraits
  ├── Customization
  ├── DailyRituals
  ├── Emblems
  ├── Favors
  ├── Perks
  ├── Help
  ├── HelpLoading
  ├── ItemAddons
  ├── Items
  ├── Packs
  ├── Powers
  └── StatusEffects
```
Fill out [this Google Form](https://docs.google.com/forms/d/e/1FAIpQLSeoz3gwXeL4Ml_ziA1u8PWeClTN1xW4ejai6iWBiVq_I4kb0w/viewform) with the following information:
- Your pack's name
- Your pack's version, including the lastest chapter it is made for
- A method of contact (Discord, Email etc)
- A direct download link to your pack
- A direct link to a banner for your pack (Imgur, etc)
- A list of people who have contributed to the pack, and (optinally) a link for each of them (to their website, twitter, etc)
- Any tags you would like your pack to have

Your pack will be checked and added to this repository if no issues are found. Automatic refreshing of the program's packs may take up to 12 hours, but it can be manually checked at any time in the settings.

## Contributing to this Repository
Packs added to this repository should be in the following json format. Valid `contains` elements can be found in the main program's `Constants` file. 
```json
{
	"name": "Pack Name",
	"chapter": 27.0,
	"packVersion": 1,
	"bannerLink": "<link>",
	"downloadLink": "<link>",
	"credits": [
		{
			"name": "Username",
			"link": "<link>"
		},
		...
	],
	"contains": ["<element>", "<element>", ...],
	"tags": ["<tag 1>", "<tag 2>", ...]
}
```
The file name should be the pack's name in lowercase, with spaces replaced with underscores and non alpha-numeric character removed.
