---
tags:
  - obsidian
image: https://images.unsplash.com/photo-1471107340929-a87cd0f5b5f3?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=300&q=80
home: /Invio/index.html
brand: Invio
slogan: Sync and Publish your docs as Website with Invio
gaID: G-039JZ5HBKZ
sort: 1
description:  This is the landing page of this site.
title: Invio - Sync and Publish with Invio
icon: https://docs.webinfra.cloud/logo.png
canonical: https://docs.webinfra.cloud/Invio/index.html
keywords:
- invio
- obsidian sync
- obsidian publish
- publish docs to website
- obsidian publish alternative
- free publish
---



## Invio - Brief Introduction


Invio provides users with a seamless workflow for synchronizing their Obsidian documents and publishing them to AWS S3 or compatible COS.

With Invio, you can automate the conversion of your documents into HTML web pages and keep them in sync across multiple devices.

![[demo2.gif]]



>[!info] Open source
>	Go to check the open sourced github repo: [Invio](https://github.com/frontend-engineering/Invio)
>


## What's New
- 0.7.22: 🔥 Show file diff view before committing.
- 0.7.12: 🔥 Fixed file path-related issues on Windows system and some bug fix.
- 0.7.5: 🔥 Fixed the issue of local image file links being lost when exporting the file.
- 0.7.2: 🔥 Support Windows platform.
- 0.6.5: 🔥 Fix an export bug that may occur in the latest version of Obsidian, where it only exports a partial portion of the Markdown file's contents instead of the entire file.
- 0.6.3: 🔥 Optimized the mobile reading experience for published sites
- 0.3.7: 🔥 Implement a differential check of the contents before syncing files.
- 0.3.5: 🔥 Added keyboard support for the search component.
- 0.3.4: 🔥 Improved support for the search component.
- 0.3.3: 🔥 Support `sort` in [metadata](https://docs.webinfra.cloud/Invio/Metadata.html) 
- 0.3.2: 🔥 Support google analytics [metadata](https://docs.webinfra.cloud/Invio/Metadata.html)
- 0.3.1: 🔥 Export / Import Settings helps to sync with co-workers [Instantly sync notes with co-workers at no cost with Invio](https://docs.webinfra.cloud/Invio/blogs/Instantly%20sync%20notes%20with%20co-workers%20at%20no%20cost%20with%20Invio.html)
- 0.3.1: 🔥 Extract all asset resources of published website from Obsidian publish hosting
- 0.3.1: 🔥 Support SEO tag `canonical` [Site Config](https://docs.webinfra.cloud/#Site_Config)
- 0.2.4: 🔥 Add right-click context menu options for files, including syncing/publishing the current file
- 0.2.3: 🔥 Add right-click context menu options for folders, including changing the working directory and syncing/publishing the current working director
- 0.2.2: 🔥 Add XML sitemap generation for improved SEO [Invio/SEO friendly|SEO friendly](https://docs.webinfra.cloud/Invio/SEO%20friendly.html)
- 0.2.1: 🔥 Support custom domain settings for a more personalized experience [Invio/Custom Domain|Custom Domain](https://docs.webinfra.cloud/Invio/Custom%20Domain.html)
- 0.2.1: 🔥 Introduce a one-click option to automatically fix failed files when an error occurs during publishing or syncing
- 0.2.0: 🔥 background notifications are handled by merging syncing and publishing workflows
- 0.2.0: 🔥 Add [StatsView](https://docs.webinfra.cloud/Invio/StatsView.html)


## Goal

Invio is a tool designed to simplify the management of your documents and seamlessly integrate them between your local device and an online website.

Invio aims to streamline document management and empower users to focus on the creative aspects of their work.

With Invio, you can enjoy the process of editing and writing without worrying about server maintenance or other technical complexities.

Invio also allows for easy sharing of configuration settings with teammates for collaboration purposes.

Invio offers SEO optimization to improve search engine indexing. Additionally, it handles conflicts in edits through a merge strategy.


## Download and  Install
- Option #1: Search **Invio** in the official "community plugin list", or visit this: https://obsidian.md/plugins?id=invio (which should redirect you into Obsidian app), then install the plugin.
- Option #2: You can also use Obsidian42 - BRAT to install this plugin. Input frontend-engineering/Invio in the configuration of BRAT.

- Option #3: [![downloads of latest version](https://img.shields.io/github/downloads/frontend-engineering/invio/total.svg)](https://github.com/frontend-engineering/Invio/releases) Manually download assets (`main.js`, `manifest.json`, `styles.css`) from the latest release.
- Option #4: [![BuildCI](https://github.com/frontend-engineering/Invio/actions/workflows/auto-build.yml/badge.svg)](https://github.com/frontend-engineering/Invio/actions/workflows/auto-build.yml) Every artifacts are placed in the "Summary" under every successful builds. It's automatically generated by every commit, may break something.


## Getting Started

After simple S3 setup, all you need to do is click the Invio ribbon icon.
[Streamlining Your Workflow with Invio](https://docs.webinfra.cloud/Invio/Streamlining%20Your%20Workflow%20with%20Invio.html)


Clicking on the ribbon icon will trigger the sync and publish process, which will be handled by Invio. You don't need to worry about anything else - just sit back and wait for the report once everything is done.

You can check the report on the right panel of the screen. This will provide you with all the information you need about the sync and publish process, including any errors or issues that may have come up. With Invio, it's easy to stay on top of your website and make sure everything is running smoothly.

## More

### Publish Report
A statistic report would show on the right sidebar when publishing.
All process details would be listed here. So you can see which files are syncing and which files are publishing.
If any job failed, it would be listed here either.

The action report is not only for running jobs review. It would show an auto-fix button if files failed to publish. Click the button, it would auto redo the jobs failed. Super useful when your network is not stable.



### Config

#### S3
To enable Invio and publish Obsidian documents to AWS S3 / Tencent Cloud Object Storage (COS), please follow these steps:

1. Prepare your COS (-compatible) service information, : [endpoint, region](https://docs.aws.amazon.com/general/latest/gr/s3.html), [access key id, secret access key](https://docs.aws.amazon.com/sdk-for-javascript/v3/developer-guide/getting-your-credentials.html), bucket name:
    
    - Endpoint: The endpoint for your COS-compatible service.
    - Region: The region where your COS bucket is located.
    - Access key ID: The access key ID associated with your COS account.
    - Secret access key: The secret access key associated with your COS account.
    - Bucket name: Create an empty bucket solely for publishing web pages.
2. Download and enable the Invio plugin in your Obsidian settings.
    
3. Enter your COS information into the settings of the Invio plugin:
    
    - Choose the local directory you want to publish.
    - Input the COS bucket information prepared in Step 1.
4. Once the setup is complete, you will see a green icon next to the chosen directory in the left file tree list.
    
5. To publish your documents to remote, click on the new icon on the ribbon (left sidebar). Alternatively, you can configure automatic synchronization in the settings panel. During the publishing process, the icon will change to "two half-circle arrows".

---
- **Be patient while publishing.** Especially in the first-time publish.
- You can even share all your config above with your teammates. You can find **Export/Import** in the settings. So your teammates don't have to input such complicated keys or secret strings.


#### Tencent Cloud (COS)

> [!note] Using Tencent Cloud(COS) example
> If you're using Tencent Cloud(COS), and your bucket region is ap-shanghai
> Your settings should be like:
> 	- **Endpoint**	cos.ap-shanghai.myqcloud.com
> 	- **Region**	ap-shanghai
> 	- **AccessKeyID**	YourSercretId
> 	- **SecretAccessKey**	YourAccessKey
> 	- **BucketName**	obsidian-123456789

To test your settings, you can click the button **check** in settings to test your COS connectivity.

### Cooperate with your teammates


Invio provides a feature that allows you to collaborate and share your configuration with teammates. By using the "Export/Import" option in the settings menu, you can easily export your configuration settings and share them with your teammates. This eliminates the need for them to input complex keys or secret strings manually.

Once your teammates have imported the shared configuration, you can all edit the documents together. Invio will sync (manual/auto) all your edits and changes, ensuring everyone has the most up-to-date version of the document.

In the case of conflicts where multiple people edit the same document simultaneously, Invio follows an ordinary merge strategy, where the latest edit takes precedence. If conflicts occur, a .conflict.md file will be automatically generated in your local folder. This file contains the remote version of the conflicted file, allowing you to manually compare and resolve the conflict.

Collaboration is made easier through Invio, enabling seamless teamwork and efficient document editing.

### Meta config


To configure the SEO settings for your published site, you can use the Meta config feature [Metadata](https://docs.webinfra.cloud/Invio/Metadata.html) in Invio. This allows you to optimize your pages for search engine indexing and improve the quality of web page retrieval.



### SEO

Before publishing your site, it's important to pay attention to SEO configuration for important pages. This will help search engines index and retrieve your web pages more effectively. You can refer to the [SEO friendly](https://docs.webinfra.cloud/Invio/SEO%20friendly.html) document for guidance on how to make your pages SEO-friendly.

By optimizing your SEO settings, you can enhance the visibility and discoverability of your published site in search engine results.


## Most Frequently Questions

The most frequently asked questions about Invio.  [Help](https://docs.webinfra.cloud/Invio/Help.html)

Or you can submit new issues [github](https://github.com/frontend-engineering/Invio/issues)

