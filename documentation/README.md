# Documentation

The documentation for this years Hackathon must be provided as a readme in Markdown format as part of your submission. 

You can find a very good reference to Github flavoured markdown reference in [this cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). If you want something a bit more WYSIWYG for editing then could use [StackEdit](https://stackedit.io/app) which provides a more user friendly interface for generating the Markdown code. Those of you who are [VS Code fans](https://code.visualstudio.com/docs/languages/markdown#_markdown-preview) can edit/preview directly in that interface too.

Examples of things to include are the following.

## Summary

**Category:** Best use of xConnect and/or Universal Tracker

What is the purpose of your module? What problem does it solve and how does it do that?

## Pre-requisites

Does your module rely on other Sitecore modules or frameworks?

- List any dependencies
- Or other modules that must be installed
- Or services that must be enabled/configured

## Installation

Provide detailed instructions on how to install the module, and include screenshots where necessary.

1. Use the Sitecore 9.1 Installation wizard to install Sitecore [package](https://dev.sitecore.net/Downloads/Sitecore_Experience_Platform/91/Sitecore_Experience_Platform_91_Initial_Release.aspx)
2. Create some pages in your Sitecore Installation 
3. Enable Experience Analytics
4. Docker up the Latest Version of UserGrid
5. Enable the MongoDB Sitecore Connector
6. Update the MongoDB xConnect Connection String to point to your UserGrid Installation
7. Browse the pages on your Sitecore Site to create Analytical data
8. Confirm data is being stored in the UserGrid\Cassandra container of the UserGrid Stack

## Configuration

How do you configure your module once it is installed? Are there items that need to be updated with settings, or maybe config files need to have keys updated?

Remember you are using Markdown, you can provide code samples too:

```xml
<?xml version="1.0"?>
<!--
  Purpose: Configuration settings for my hackathon module
-->
<configuration xmlns:patch="http://www.sitecore.net/xmlconfig/">
  <sitecore>
    <settings>
      <setting name="MyModule.Setting" value="Hackathon" />
    </settings>
  </sitecore>
</configuration>
```

## Usage

How does the end user use the Module?


## Video

Please provide a video highlighing your Hackathon module submission and provide a link to the video. Either a [direct link](https://www.youtube.com/watch?v=EpNhxW4pNKk) to the video, upload it to this documentation folder or maybe upload it to Youtube...

[![Sitecore Hackathon Video Embedding Alt Text](https://img.youtube.com/vi/EpNhxW4pNKk/0.jpg)](https://www.youtube.com/watch?v=EpNhxW4pNKk)
