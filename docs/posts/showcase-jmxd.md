---
title: "Community Showcase: jmxd Overlays"
date:
  created: 2024-09-19
authors:
  - yozora
categories:
  - Showcase
---

![jmxd preview image](../images/jmxd-preview.png){ align=right itemprop="image" }

## **Showcasing Community Creations: jmxd’s Overlays for Kometa**

We’re excited to kick off what we hope will be the first of many showcases of incredible, community-driven creations. Today, we shine a spotlight on the amazing work of [jmxd](https://github.com/jmxd/Kometa), who has designed some stunning overlays for Kometa users.

A long-time member of the [Kometa Discord Server](https://kometa.wiki/en/latest/discord/), jmxd has been hard at work developing overlays based on media information (such as resolution and edition) and audience ratings. After much anticipation, these overlays are now available for the community to enjoy!

Read on to discover more about jmxd’s impressive work and how you can integrate these overlays into your own setup!

<!-- more -->

### **Introducing jmxd’s Overlays**

jmxd has crafted two modular overlay files, which can be used individually or—our recommendation—together for the best experience.

The first overlay displays the current audience rating from your Plex server. The rating is shown with a color-coded scale: green for ratings 8+, yellow for 6-7, and red for anything below 6.

The second overlay provides detailed media info such as resolution, edition, video, and audio formats. These overlays are designed to be minimalistic, streamlined, and easy on the eyes.

Here are some examples of jmxd’s overlays in action:

![jmxd image 1](https://camo.githubusercontent.com/495ef118b3aad3acaaa98042a2a6f7ba93218d927330006fb164ecab7752db01/68747470733a2f2f692e696d6775722e636f6d2f78674576324f652e706e67)

### **Important Notes**

Full documentation for these overlays is available in [jmxd’s GitHub repository](https://github.com/jmxd/Kometa).

- These overlays are designed to work seamlessly with the [TRaSH Naming Conventions](https://trash-guides.info/Radarr/Radarr-recommended-naming-scheme/#plex), a popular file-naming convention for Plex users.
- Only high-quality media (1080p and above) will display the resolution overlay. Anything below 1080p is excluded.
- Dolby Vision with HDR/HDR10+ fallback support is detected and matched separately from exclusive DV, but only the Dolby Vision label will be shown. See examples at the bottom for alternative options.
- These overlays are compatible with media at the Movie, Show, and Episode levels.

### **How to Use the Overlays**

To use jmxd’s overlays, head over to the [GitHub repository](https://github.com/jmxd/Kometa). Click the green "Code" button and select "Download ZIP". Extract the contents of the ZIP file and place them in the folder mapped to `config` within Kometa.

Next, to enable the overlays, add the following to your `config.yml` file (replacing `LIBRARYNAMEHERE` with the name of your library):

```yaml
libraries:
  LIBRARYNAMEHERE:
    overlay_files:
      - file: config/overlays/media_info.yml
      - file: config/overlays/audience_rating.yml
```

There are several customizable variables (such as enabling/disabling specific parts of the overlays), which you can modify using template variables. Full details are available on the [GitHub repository](https://github.com/jmxd/Kometa).

For questions, support, or to thank jmxd, check out the dedicated [Discord thread](https://discord.com/channels/822460010649878528/1248134055527059496).

A huge thank you to jmxd for this fantastic contribution! We look forward to sharing more community creations in the future.

