# Gphotos-Takeout-fixer
A series of scripts that are ideally intended to merge JSON metadata with their respective photos downloaded from Google Photos takeout, with some manual touches.

## 🚀 Inspiration
When we tend to download all the photos that are backed-up by Google Photos, there is a service provided by Google itself to make the process much easier. That is called [**Google Takeout**](https://takeout.google.com). But there is a problem with this approach:  
  
- The changes that we do to the files when they are in online Google server won't be saved to the files itself.  
- For example if you add a location or changed the date taken of any particular photo/video 🖼️, it'll be saved as separate metadata in servers & appears only in Google Photos website or client.
- So if you download any file locally all the changes you made are lost.
- But when you decided to download all your Google Photos through Takeout feature, the metadata is provided in a separate **JSON** files 📜.
- Hence we are assured that our metadata isn't completely lost.  
  
But this doesn't solve our problem. Although we may have the metadata but there is no simply way to merge all the metadata that is present is JSON files to its respective photos/videos. Hence through this project we are trying to fix that.
  
## ℹ️ Basic Info  
This section tries to provide some knowledge with the terms involved in this project (these is necessary stuff that helps you understand the project easier).

1. **Whats is metadata/exifdata?**  
Metadata or in other words EXIF data is a series of tags with certain values/data that is present the file along with the media. This includes a long list of tags/properties which include: Date taken, Location coordinates, Device used etc.  
  
2. **Does every file has metadata?**  
While most of the modern day devices embed certain amount of metadata to every image or video captured - but that doesn't mean media files can't exist without metadata. We can add, edit or remove metadata tags. Example:
