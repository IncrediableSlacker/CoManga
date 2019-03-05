# Supported Platforms/OS
CoManga supports :
* Android
* iOS
* UWP

# Contribution
Contributing to the project is fairly simple. I'd recommend going through the project structure first thoroughly. As you can see, CoManga is divided into 2 sections, i.e., Comic and Manga. The respective code will go in the provided directories. Please keep in mind that you follow these points :
- Update the "Changelog.md" and "Changelog.txt" in the specified format. Even if it is a small typo fix or an issue fixed.
- Every method you create should have your Github username in this format : @Xonshiz (Xonshiz is my Github Handle)
- Please try to comment the logic wherever possible you're applying because a fellow developer might not understand what you did and why you did it.
- Whatever functionality you add, please make sure that it runs on every platform. The UI may not be pixel perfect, that's fine.

## Opening An Issue/Requesting A Site
If your're planning to open an issue for the script or ask for a new feature or anything that requires opening an Issue, then please do keep these things in mind.

### Reporting Issues
If you're going to report an issue, then please make sure that the application has all the necessary permissions granted and you're connected to a stable internet connection and you have enough storage space.

Please upload a screenshot of the issue, if possible. Please follow this syntax :

**What You're Trying To Download** : Comic Or Manga

**What Went Wrong?** : What happened?

**Your Device's Operating System** : What OS are you on? Android, iOS or UWP.

**Version Number of Application** : Check from the "Settings" Tab and post it here.
 
### Suggesting A Feature
First things first, please don't make suggestions for these things, as they are already in progress or I have plans of adding them in the application in future.
- Download all the chapters.
- Sorting the chapter list.
- Downloading chapters in a particular range. For Eg : Download 11-16 chapters of a comic/manga.

I don't mean to be rude, but it's such a drag to see the requests for same things over and over again. Please understand. So, if I see any request for either of these things, I'll close the issue immidiately.
However, if you have suggestions on what can be added to these functionalities, please open an issue for the same.

If you're here to make suggestions, please follow the basic syntax to post a request :

**Subject** : Something that briefly tells us about the feature.

**Long Explanation** : Describe in details what you want and how you want.

This should be enough, but it'll be great if you can add more ;)

# Where to download from?
Currently, you can download the builds/packages from the [Latest Releases](https://github.com/Xonshiz/Comic_dl-Mobile-Application/releases/latest) Section only. I do have future plans to push this to various application stores.

# Why is it not on application stores?
I have plans on putting these on Play Store (Android), Windows App Store and iOS Application Center. But, currently I do not have that kind of money to invest in all of these together. Hopefully by April 2019 end, I'll push this to Google Play Store and Windows Store as well. iOS is costly AF and will take time...A LOT OF TIME. WHY U DO THIS APPLE?!

# Download Locations?
Since Xamarin Forms is a cross-platform app. developement framework, there are certain things that you need to do platform dependently and getting correct write permissions to save files and creating directories in custom locations is a little tricky. At least it is for me. So, I'm learning along the way and over the time, you'll definitely get a better experience. So, these are some locations you can find your downloaded Comics/Manga. Check the platform-wise locations :
![iOS Build](https://github.com/Xonshiz/Comic_dl-Mobile-Application/blob/master/OnlineAssets/macOS_Build.gif?raw=true)

#### Android
You need to browse to your device's "Internal Storage" and there you'll see a folder named "Comic_DL". Inside that folder you'll find your Comics/Manga under their own respective folders.

#### iOS
If you're on iOS, then you're compiling the project and the files will be stored in temp folders of the Simulator. There are multiple steps to this. First, make sure you sort all the folders based on "Last Modified". After that, go to this location :
`/Users/{YourUserName}}/Library/Developer/CoreSimulator/Devices/{SortedFolderOnTop}/data/Containers/Data/Application/{SortedFOlder2OnTop}/Documents/Pictures/`

You should get your downloaded items there.

#### UWP
Getting the permissions is a little tricky in UWP. I've literally tried a lot of different things and couldn't get it to work. So, you'll have to work hard to get these downloaded files. You can find them in this location :
`Put UWP Location Here`

# How To Compile
Install Visual Studio (Recommended Version : 2017). You can install Visual Studio Community version as well, it'll work just fine. Open this project in Visual Studio. Depending upon your device OS, follow these steps :
#### Android
#### iOS
If you have an iPhone, connect it to your device via wires (however iPhones are connected to a system). Or, if you don't have an iPhone, you need macOS to build this. You'll also need to install and updated "XCODE". Then follow this .gif :

#### UWP

# Installing Apps
For installing the application on respective OS, follow the guides below.
#### Android
Download the "CoManga.apk" from the [Latest Releases](https://github.com/Xonshiz/Comic_dl-Mobile-Application/releases/latest) section and install as you would install any other apk. You might have to switch on [Allow App Installations From Third Party Vendor](http://www.inbox.com/article/how-do-enable-third-party-apps-on-android.html).
It's as easy as that.

#### iOS
Currently there's no build for iOS. So, you'll have to compile the project yourself. Check the "How To Compile" section for details.

#### UWP
UWP app is also available in the [Latest Releases](https://github.com/Xonshiz/Comic_dl-Mobile-Application/releases/latest) section. You can download the application from there and run it like any other application.

# Special Permissions
Since the application connects to internet and stores files on your system's hard disk, it needs certain permissions from the user. Find the permissions and their usages below :

#### Android
INTERNET : To access the internet.
STORAGE : To store files on the disk.

#### iOS
Calender : Due to apple's policies, we need this. One of the dependency in the application has made this permission necessary. Though, that plugin and this application doesn't use any of this.

#### UWP
Documents Library, Downloads, Pictures : Trying to store the data.

# Known Issues, Workarounds...
Sometimes you'll click the download button and then it'll show "Downloaded" with a blank message. You might have to try to download again. If the problem persists, please feel free to open an issue.

# Why no iOS build? Why do I have to go through such a pain?
I'll break it down in a very very simple manner. I need to have a developer account to be able to push this application to stores. These are the charges for a developer account on these 3 platforms :
* Android : Google Play Store => $25 Lifetime
* Windows Store (UWP) => $19 Lifetime
* iOS App. Store => **$100 PER YEAR** (For Single Developers).

So, I do not make that kind of money and I hope you got the picture why this is not on iOS Stores. Plus, you need an apple device to build the distributable package. I use a Lenovo Laptop for god's sake. But, borrowing a Mac shouldn't be THAT hard, getting the money for the iOS developer account is though.

# Why Xamarin.Forms?
I've been working with Xamarin.Forms for over an year now and I like it. Despite of a lot of weird errors and bugs and some other annoying things, I love it. It just easy to grasp and work with. The community support is decent enough now. If you're a Xamarin Developer, you'd understand. And if you're a Xamarin Developer who start 2-4 years ago, you know the pain.
Anyways, the main point was that Xamarin.Forms is a "Cross-Platform" Mobile Developement Framework. So, write in 1 language (C#) and deliver application on 3 platforms, namely, Android, iOS and UWP (Windows 10), while sharing the single code base. Go on and Google it, that'll give you a better idea.

# Manga and Comic Sources?
The current application takes ["MangaRock"](https://mangarock.com/) as a source for Manga and ["ReadComicsOnline.Me"](https://readcomicsonline.me/) as a source for fetching Comics. These are subjected to change if anything goes down or there some issue. But, for now, we'll go with these two. I initially wanted to go with ["Readcomiconline.To"](https://readcomiconline.to/) as a source for Comics, but it runs behind CloudFlare and it's a hassle to bypass it. Sure, comic-dl cli implements it and thanks to anorov's cf-scrape, it all works. But, it's not a C# based solution. And Believe me, if you've worked with Xamarin, it's a real hassle to deal with a lot of times. So, in short, I didn't want to over complicate things with CloudFlare, so in the end, I went with ReadComicsOnline.Me as a source for comics.

# What if I want to download from somewhere else?
Currently there is no such functionality in this version of the application. However, in the future, I have plans of adding this functionality. It might be limited, but it'll be there. For now, you can directly search your required Comic or Manga from the Search Bar in the respective sections and download the comics. If for some reason, the comic/manga you're looking for is not available on either of the platforms, you can head to comic-dl cli.

# How long till we can download from custom websites?
No Clue. Could be next week, could be next month, or could be next year. Depends on the amount of time I have and the motivation I have to work on this. Btw, you're all welcome to pull this, work on it and send Pull Requests.

# Why Ads?
So, this was a big decision for me to make. If you read the "Why No iOS Build?" section, you'll see that I need money to get an iOS developer account. Donations are always open, but I do need some extra cash and donations aren't much. So, I'll try to save and invest some in it. Don't worry, as the advertisements are just small banners. I promise that no ad will "pop up" or get in your way. I understand it's annoying. So, you will NEVER get those kinds of ads, if you use from this source.
