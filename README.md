This is the repository for submitting datapacks to dManager.
Read more about dManager here: [stevertus.ga/dManager](http://stevertus.ga/dManager)


In this guide you will learn how to setup your datapack for a submission and where to submit it then.

Maybe you did already notice it: dManager has a version system that allows it to send updates to the users. So you have to invest a bit more effort to setup your files properly.

I would suggest that you call your releases like the version (e.g: tekPack v0.3.zip).

So you and the consumer know which version is used.

dManager **does not** host the files! It provides just the platform and the connection to the files.

I would consider uploading these files to gitHub, nofile.io or your own web source. It is important that these files can be accessed directly without loading a website!

You need a setup json file for your datapack. All the possible values are explained below.
Luckily I made a generator for this further [here](http://stevertus.ga/dManager/submit), so it should not be that hard.

> [] is optional

```
{
  "id":"your unique pack id",
  "type":"datapack or resourcepack",
  "version":"latest version (I suggest a format like 0.1.3)",
  "title":"the displayed title",
  "logo":"a logo or small image for the pack (must be square)",
  ["video"]:"link to a youtube video",
  ["url"]: "a base url to your project (all other urls can be
			shortened by beginning with /)"
  ["banner"]: "a banner image for the details page",
  ["creator"]: "name of the creator",
  ["creatorLink"]: "a link to social media or whatever",
  ["website"]: "a link to a website for datapacks or to a post",
  "files": {
	// list here for every past version the download link(full)
    "0.2": "http://download.com/version v0.2.zip",
    "0.1": "http://download.com/version v0.1.zip"
  },
  "description":"a link directly to a markdown or basic html file
   				       that describe the datapack and how to use it",
  ["dependencies"]:[
	"an array of all the ids of packs your pack requires",
	"e.g: utils, libaries, own resource pack",
	"great to ship a resource pack right with the datapack"
]
}

```
If you filled out the form below or made your own json you are ready to publish it! I want to have a high quality selection of datapacks in dManager, so every submitted pack is checked manually, so it can take a few days until it is released.

You can publish your datapack in different ways:
* use the submit button in the app or [here](http://stevertus.ga/dManager/submit)
* create a pull request on gitHub: [here](https://github.com/Stevertus/dManager-packages/pulls)
* write a message on my [Discord](https://discord.gg/BmnMBSq) in the channel #feature-my-pack
* contact me by email [stevertusyt@gmail.com](mailto::stevertusyt@gmail.com)


If you have further questions, contact me with one of the options obove.
