*Note*: `user` and `key` are essential as query parameters for all API endpoints. 

# API Response sample

##### GET `beta/campaigns/?cuid=12175&state=running&stats=true&legacy=false&user=<USER_EMAIL>&key=<KEY>`

```json
{
  "ancestors": [
    {
      "HasContract": true,
      "ID": 51,
      "level": "wl",
      "name": "Metroland Digital"
    },
    {
      "Currency": "CAD",
      "ID": 12175,
      "Wallet": null,
      "level": "customer",
      "name": "1477462_Terra Greenhouses "
    }
  ],
  "campaigns": [
    {
      "CampCode": 37054,
      "DaysLeft": 23,
      "EndDate": "2017-05-03 23:59:00",
      "Name": "dev Terra Greenhous",
      "StartDate": "2017-04-06 00:00:00",
      "TimeZone": "America/Toronto",
      "TotalActions": 0,
      "TotalClicks": 0,
      "TotalDays": 28,
      "TotalImpressions": 0,
      "TotalSpend": 0,
      "delivery": [
        {
          "Actions": 0,
          "Clicks": 0,
          "Date": "2017-04-06",
          "Impressions": 0,
          "Spend": 0
        }
      ],
      "delivery_avg": {
        "Actions": 0,
        "Clicks": 0,
        "Impressions": 0,
        "Spend": 0
      }
    }
  ]
}
```

##### GET `beta/campaigns/37054?summary=true&incurrency=true&user=<USER_EMAIL>&key=<KEY>`

```json
{
  "ancestors": [
    {
      "ID": 51,
      "level": "wl",
      "name": "Metroland Digital"
    },
    {
      "ID": 12175,
      "level": "customer",
      "name": "1477462_Terra Greenhouses "
    }
  ],
  "metadata": {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37054,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": true,
    "EndDate": "2017-05-03 23:59:00",
    "Language": null,
    "LastUpdated": "2017-04-11 10:35:31.2930000",
    "Level": "offer",
    "Name": "Terra Greenhouses_71022_April-May/17_Programmatic",
    "OfferCategories": "IAB10",
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 0,
    "SelfServe": true,
    "StartDate": "2017-04-06 00:00:00",
    "TimeZone": "America/Toronto"
  },
  "summary": {
    "Revenue": 77.688,
    "children": 37054,
    "clicks": 44,
    "impressions": 38844
  }
}
```

##### GET `beta/campaigns/37057/banners?cuid=12175&user=<USER_EMAIL>&key=<KEY>`

```json
[
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79628,
    "BannerName": "TERRA_BigBox_300x250_SPRINGCLEAN_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_BigBox_300x250_SPRINGCLEAN_Apr6_12.6dd2d04ec9eb4cc59a601ccdef51d2b6.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=BigBox300x250&utm_content=SPRINGCLEAN&utm_campaign=0406017",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79628 - TERRA_BigBox_300x250_SPRINGCLEAN_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=BigBox300x250&utm_content=SPRINGCLEAN&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 300,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 11
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79629,
    "BannerName": "TERRA_DblSkyscraper_300x600_PLANTER_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_PLANTER_Apr6_12.5e760f75668a46bca0e03e944c56be93.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=DblSkyscraper300x600&utm_content=PLANTER&utm_campaign=0406017",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79629 - TERRA_DblSkyscraper_300x600_PLANTER_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=DblSkyscraper300x600&utm_content=PLANTER&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 300,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 13
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79630,
    "BannerName": "TERRA_MobileBanner_300x250_EASTER_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraEaster_Apr_300x250_70063.9ac1d1fe407b46d582c298452747b65d.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=BigBox300x250&utm_content=EASTER&utm_campaign=0406017",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79630 - TERRA_MobileBanner_300x250_EASTER_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=BigBox300x250&utm_content=EASTER&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 300,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 11
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79631,
    "BannerName": "TERRA_MobileBanner_300x50_EASTER_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraEaster_Apr_320x50_70063.44da354f7dfc4374856fc8a410e3d47c.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=MobileBanner300x50&utm_content=EASTER&utm_campaign=0406017",
    "GoogleAuditResult": "PENDING_REVIEW",
    "GoogleCreativeID": "79631 - TERRA_MobileBanner_300x50_EASTER_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 50,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=MobileBanner300x50&utm_content=EASTER&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 320,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 167
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79632,
    "BannerName": "TERRA_Leaderboard_728X90_EASTER_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraEaster_Apr_728x90_70063.f95d395730ec47a681a2ee9e0c4538fa.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=Leaderboard728x90&utm_content=EASTER&utm_campaign=0406017",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79632 - TERRA_Leaderboard_728X90_EASTER_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 90,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=Leaderboard728x90&utm_content=EASTER&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 728,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 1
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79633,
    "BannerName": "TERRA_BigBox_300x250_PLANTER_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraPlanter_Apr_300x250_70063.17d5e7ca1f2045a68b4b9e52e9826559.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=BigBox300x250&utm_content=PLANTER&utm_campaign=0406017",
    "GoogleAuditResult": "PENDING_REVIEW",
    "GoogleCreativeID": "79633 - TERRA_BigBox_300x250_PLANTER_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=BigBox300x250&utm_content=PLANTER&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 300,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 11
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79634,
    "BannerName": "TERRA_Leaderboard_728X90_PLANTER_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraPlanter_Apr_728x90_70063.ac19107a726947c78efc1c295b2f81bc.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=Leaderboard728x90&utm_content=PLANTER&utm_campaign=0406017",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79634 - TERRA_Leaderboard_728X90_PLANTER_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 90,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=Leaderboard728x90&utm_content=PLANTER&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 728,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 1
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79649,
    "BannerName": "TERRA_Leaderboard_728X90_SPRINGCLEAN_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_Leaderboard_728X90_SPRINGCLEAN_Apr6_12.84283807fc4b45a397ecf53b7ce5cb34.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=Leaderboard728x90&utm_content=SPRINGCLEAN&utm_campaign=0406017",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79649 - TERRA_Leaderboard_728X90_SPRINGCLEAN_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 90,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=Leaderboard728x90&utm_content=SPRINGCLEAN&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 728,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 1
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79664,
    "BannerName": "TERRA_DblSkyscraper_300x600_EASTER_Apr6_12_",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_EASTER_Apr6_12.743bab0de3ed43329832b3dc94de23bb.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=DblSkyscraper300x600&utm_content=EASTER&utm_campaign=0406017",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79664 - TERRA_DblSkyscraper_300x600_EASTER_Apr6_12_",
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=DblSkyscraper300x600&utm_content=EASTER&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 300,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 13
  },
  {
    "AdvertiserId": 12176,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79665,
    "BannerName": "TERRA_DblSkyscraper_300x600_SPRINGCLEAN_Apr6_12",
    "BannerType": 2,
    "Brand": "",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_SPRINGCLEANApr6_12.ec13df027a744861b3fd7075a9f7a3d8.jpg",
    "FinalUrl": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=DblSkyscraper300x600&utm_content=SPRINGCLEAN&utm_campaign=0406017",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79665 - TERRA_DblSkyscraper_300x600_SPRINGCLEAN_Apr6_12",
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgLink": "http://www.terragreenhouses.com/specials/?utm_source=Spec&utm_medium=Online&utm_term=DblSkyscraper300x600&utm_content=SPRINGCLEAN&utm_campaign=0406017",
    "ImgTarget": "_blank",
    "ImgWidth": 300,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 13
  }
]
```

##### GET `beta/campaigns/37054/children?level=offer&summary=true&incurrency=true&user=<USER_EMAIL>&key=<KEY>`

```json
[
  {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37055,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": true,
    "EndDate": "2017-04-12 23:59:00",
    "FlightID": 0,
    "Language": null,
    "LastUpdated": "2017-04-10 14:53:05.8630000",
    "Name": "Terra Greenhouses_71022_April6-12_BB+DSS+LB_Behavior",
    "OfferCategories": null,
    "OfferID": 37054,
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 2,
    "SelfServe": true,
    "StartDate": "2017-04-06 00:00:00",
    "TimeZone": "America/Toronto",
    "summary": {
      "Actions": 0,
      "Clicks": 37,
      "Impressions": 37369,
      "Revenue": 74.738
    }
  },
  {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37062,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": true,
    "EndDate": "2017-04-12 23:59:00",
    "FlightID": 0,
    "Language": null,
    "LastUpdated": "2017-04-10 08:37:43.2670000",
    "Name": "Terra Greenhouses_71022_April6-12_MB+BB_GEO",
    "OfferCategories": null,
    "OfferID": 37054,
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 2,
    "SelfServe": true,
    "StartDate": "2017-04-06 00:00:00",
    "TimeZone": "America/Toronto",
    "summary": {
      "Actions": 0,
      "Clicks": 47,
      "Impressions": 36735,
      "Revenue": 73.47
    }
  },
  {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37132,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": true,
    "EndDate": "2017-04-19 23:59:00",
    "FlightID": 0,
    "Language": null,
    "LastUpdated": "2017-04-11 13:20:12.2670000",
    "Name": "Terra Greenhouses_71022_April13-19_BB+DSS+LB_Behavior",
    "OfferCategories": null,
    "OfferID": 37054,
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 2,
    "SelfServe": true,
    "StartDate": "2017-04-06 00:00:00",
    "TimeZone": "America/Toronto",
    "summary": {
      "Actions": 0,
      "Clicks": 0,
      "Impressions": 0,
      "Revenue": 0
    }
  },
  {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37135,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": false,
    "EndDate": "2017-04-26 23:59:00",
    "FlightID": 0,
    "Language": null,
    "LastUpdated": "2017-04-11 10:22:34.1500000",
    "Name": "Terra Greenhouses_71022_April20-26_BB+DSS+LB_Behavior",
    "OfferCategories": null,
    "OfferID": 37054,
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 2,
    "SelfServe": true,
    "StartDate": "2017-04-20 00:00:00",
    "TimeZone": "America/Toronto",
    "summary": {
      "Actions": null,
      "Clicks": null,
      "Impressions": null,
      "Revenue": null
    }
  },
  {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37138,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": false,
    "EndDate": "2017-05-03 23:59:00",
    "FlightID": 0,
    "Language": null,
    "LastUpdated": "2017-04-11 10:26:20.6570000",
    "Name": "Terra Greenhouses_71022_April27-May3_BB+DSS+LB_Behavior",
    "OfferCategories": null,
    "OfferID": 37054,
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 2,
    "SelfServe": true,
    "StartDate": "2017-04-27 00:00:00",
    "TimeZone": "America/Toronto",
    "summary": {
      "Actions": null,
      "Clicks": null,
      "Impressions": null,
      "Revenue": null
    }
  },
  {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37141,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": true,
    "EndDate": "2017-04-19 23:59:00",
    "FlightID": 0,
    "Language": null,
    "LastUpdated": "2017-04-11 13:24:13.3930000",
    "Name": "Terra Greenhouses_71022_April13-19_MB+BB_GEO",
    "OfferCategories": null,
    "OfferID": 37054,
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 2,
    "SelfServe": true,
    "StartDate": "2017-04-13 00:00:00",
    "TimeZone": "America/Toronto",
    "summary": {
      "Actions": 0,
      "Clicks": 0,
      "Impressions": 0,
      "Revenue": 0
    }
  },
  {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37144,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": false,
    "EndDate": "2017-04-26 23:59:00",
    "FlightID": 0,
    "Language": null,
    "LastUpdated": "2017-04-11 10:31:24.1030000",
    "Name": "Terra Greenhouses_71022_April20-26_MB+BB_GEO",
    "OfferCategories": null,
    "OfferID": 37054,
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 2,
    "SelfServe": true,
    "StartDate": "2017-04-20 00:00:00",
    "TimeZone": "America/Toronto",
    "summary": {
      "Actions": null,
      "Clicks": null,
      "Impressions": null,
      "Revenue": null
    }
  },
  {
    "ActionLookback": 2,
    "ActionType": null,
    "AdvertiserId": 12176,
    "AgencyPercentage": null,
    "CPAReqClick": true,
    "CampCode": 37147,
    "Currency": "CAD",
    "Draft": false,
    "Enabled": false,
    "EndDate": "2017-05-03 23:59:00",
    "FlightID": 0,
    "Language": null,
    "LastUpdated": "2017-04-11 10:34:45.5000000",
    "Name": "Terra Greenhouses_71022_April27-May3_MB+BB_GEO",
    "OfferCategories": null,
    "OfferID": 37054,
    "OptimizedCampCode": 0,
    "RevType": 1,
    "Revenue": 2,
    "SelfServe": true,
    "StartDate": "2017-04-27 00:00:00",
    "TimeZone": "America/Toronto",
    "summary": {
      "Actions": null,
      "Clicks": null,
      "Impressions": null,
      "Revenue": null
    }
  }
]
```

##### GET `beta/campaigns/37057/screenshots?user=<USER_EMAIL>&key=<KEY>`

```json
[
  {
    "BannerCode": 79628,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_BigBox_300x250_SPRINGCLEAN_Apr6_12.6dd2d04ec9eb4cc59a601ccdef51d2b6.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79628_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79628_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 224,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 101,
        "TLD": "addictinggames.com"
      },
      {
        "Frequency": 73,
        "TLD": "mediatakeout.com"
      },
      {
        "Frequency": 622,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 556,
        "TLD": "kijiji.ca"
      }
    ],
    "updated": 1491956287417
  },
  {
    "BannerCode": 79630,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraEaster_Apr_300x250_70063.9ac1d1fe407b46d582c298452747b65d.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79630_37057_ebay.ca.pdf",
    "TLD": "ebay.ca",
    "_id": "79630_37057_ebay.ca",
    "domains": [
      {
        "Frequency": 205,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 234,
        "TLD": "thesportster.com"
      },
      {
        "Frequency": 832,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 563,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 217,
        "TLD": "thetalko.com"
      }
    ],
    "updated": 1491992484094
  },
  {
    "BannerCode": 79632,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraEaster_Apr_728x90_70063.f95d395730ec47a681a2ee9e0c4538fa.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 90,
    "ImgWidth": 728,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79632_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79632_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 162,
        "TLD": "mangahere.co"
      },
      {
        "Frequency": 89,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 148,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 338,
        "TLD": "zoo.com"
      },
      {
        "Frequency": 1462,
        "TLD": "kijiji.ca"
      }
    ],
    "updated": 1491938340536
  },
  {
    "BannerCode": 79633,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraPlanter_Apr_300x250_70063.17d5e7ca1f2045a68b4b9e52e9826559.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79633_37057_mediatakeout.com.pdf",
    "TLD": "mediatakeout.com",
    "_id": "79633_37057_mediatakeout.com",
    "domains": [
      {
        "Frequency": 67,
        "TLD": "mediatakeout.com"
      },
      {
        "Frequency": 179,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 531,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 480,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 74,
        "TLD": "thetalko.com"
      }
    ],
    "updated": 1491927197152
  },
  {
    "BannerCode": 79634,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraPlanter_Apr_728x90_70063.ac19107a726947c78efc1c295b2f81bc.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 90,
    "ImgWidth": 728,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79634_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79634_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 171,
        "TLD": "mangahere.co"
      },
      {
        "Frequency": 323,
        "TLD": "zoo.com"
      },
      {
        "Frequency": 143,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 1456,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 91,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491945272797
  },
  {
    "BannerCode": 79649,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_Leaderboard_728X90_SPRINGCLEAN_Apr6_12.84283807fc4b45a397ecf53b7ce5cb34.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 90,
    "ImgWidth": 728,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79649_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79649_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 122,
        "TLD": "mangahere.co"
      },
      {
        "Frequency": 89,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 125,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 1407,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 284,
        "TLD": "zoo.com"
      }
    ],
    "updated": 1491923713100
  },
  {
    "BannerCode": 79630,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraEaster_Apr_300x250_70063.9ac1d1fe407b46d582c298452747b65d.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79630_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79630_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 167,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 576,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 555,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 67,
        "TLD": "mediatakeout.com"
      },
      {
        "Frequency": 94,
        "TLD": "addictinggames.com"
      }
    ],
    "updated": 1491948539466
  },
  {
    "BannerCode": 79633,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraPlanter_Apr_300x250_70063.17d5e7ca1f2045a68b4b9e52e9826559.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79633_37057_addictinggames.com.pdf",
    "TLD": "addictinggames.com",
    "_id": "79633_37057_addictinggames.com",
    "domains": [
      {
        "Frequency": 73,
        "TLD": "addictinggames.com"
      },
      {
        "Frequency": 731,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 543,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 213,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 84,
        "TLD": "thetalko.com"
      }
    ],
    "updated": 1491963075321
  },
  {
    "BannerCode": 79649,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_Leaderboard_728X90_SPRINGCLEAN_Apr6_12.84283807fc4b45a397ecf53b7ce5cb34.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 90,
    "ImgWidth": 728,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79649_37057_lolking.net.pdf",
    "TLD": "lolking.net",
    "_id": "79649_37057_lolking.net",
    "domains": [
      {
        "Frequency": 772,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 20,
        "TLD": "lolking.net"
      },
      {
        "Frequency": 27,
        "TLD": "mangahere.co"
      },
      {
        "Frequency": 30,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 32,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491826140297
  },
  {
    "BannerCode": 79664,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_EASTER_Apr6_12.743bab0de3ed43329832b3dc94de23bb.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79664_37057_lolking.net.pdf",
    "TLD": "lolking.net",
    "_id": "79664_37057_lolking.net",
    "domains": [
      {
        "Frequency": 12,
        "TLD": "shmoop.com"
      },
      {
        "Frequency": 4,
        "TLD": "bibme.org"
      },
      {
        "Frequency": 5,
        "TLD": "drudgereport.com"
      },
      {
        "Frequency": 4,
        "TLD": "lolking.net"
      },
      {
        "Frequency": 30,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491873757051
  },
  {
    "BannerCode": 79628,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_BigBox_300x250_SPRINGCLEAN_Apr6_12.6dd2d04ec9eb4cc59a601ccdef51d2b6.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79628_37057_mediatakeout.com.pdf",
    "TLD": "mediatakeout.com",
    "_id": "79628_37057_mediatakeout.com",
    "domains": [
      {
        "Frequency": 552,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 68,
        "TLD": "mediatakeout.com"
      },
      {
        "Frequency": 206,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 568,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 94,
        "TLD": "addictinggames.com"
      }
    ],
    "updated": 1491930667403
  },
  {
    "BannerCode": 79633,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraPlanter_Apr_300x250_70063.17d5e7ca1f2045a68b4b9e52e9826559.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79633_37057_ebay.ca.pdf",
    "TLD": "ebay.ca",
    "_id": "79633_37057_ebay.ca",
    "domains": [
      {
        "Frequency": 253,
        "TLD": "thetalko.com"
      },
      {
        "Frequency": 548,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 268,
        "TLD": "thesportster.com"
      },
      {
        "Frequency": 980,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 227,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491992484095
  },
  {
    "BannerCode": 79665,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_SPRINGCLEANApr6_12.ec13df027a744861b3fd7075a9f7a3d8.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79665_37057_lolking.net.pdf",
    "TLD": "lolking.net",
    "_id": "79665_37057_lolking.net",
    "domains": [
      {
        "Frequency": 2,
        "TLD": "zoo.com"
      },
      {
        "Frequency": 3,
        "TLD": "shmoop.com"
      },
      {
        "Frequency": 2,
        "TLD": "screenrant.com"
      },
      {
        "Frequency": 8,
        "TLD": "lolking.net"
      },
      {
        "Frequency": 10,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491830432817
  },
  {
    "BannerCode": 79628,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_BigBox_300x250_SPRINGCLEAN_Apr6_12.6dd2d04ec9eb4cc59a601ccdef51d2b6.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79628_37057_addictinggames.com.pdf",
    "TLD": "addictinggames.com",
    "_id": "79628_37057_addictinggames.com",
    "domains": [
      {
        "Frequency": 92,
        "TLD": "addictinggames.com"
      },
      {
        "Frequency": 194,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 67,
        "TLD": "mediatakeout.com"
      },
      {
        "Frequency": 552,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 545,
        "TLD": "ebay.ca"
      }
    ],
    "updated": 1491927197151
  },
  {
    "BannerCode": 79629,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_PLANTER_Apr6_12.5e760f75668a46bca0e03e944c56be93.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79629_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79629_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 106,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 19,
        "TLD": "wikia.com"
      },
      {
        "Frequency": 59,
        "TLD": "topix.com"
      },
      {
        "Frequency": 43,
        "TLD": "imgur.com"
      },
      {
        "Frequency": 25,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491963075320
  },
  {
    "BannerCode": 79633,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraPlanter_Apr_300x250_70063.17d5e7ca1f2045a68b4b9e52e9826559.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79633_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79633_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 546,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 226,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 254,
        "TLD": "thesportster.com"
      },
      {
        "Frequency": 924,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 208,
        "TLD": "thetalko.com"
      }
    ],
    "updated": 1491970909631
  },
  {
    "BannerCode": 79630,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraEaster_Apr_300x250_70063.9ac1d1fe407b46d582c298452747b65d.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79630_37057_addictinggames.com.pdf",
    "TLD": "addictinggames.com",
    "_id": "79630_37057_addictinggames.com",
    "domains": [
      {
        "Frequency": 90,
        "TLD": "addictinggames.com"
      },
      {
        "Frequency": 538,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 144,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 495,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 63,
        "TLD": "therichest.com"
      }
    ],
    "updated": 1491923713100
  },
  {
    "BannerCode": 79665,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_SPRINGCLEANApr6_12.ec13df027a744861b3fd7075a9f7a3d8.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79665_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79665_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 96,
        "TLD": "topix.com"
      },
      {
        "Frequency": 42,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 76,
        "TLD": "imgur.com"
      },
      {
        "Frequency": 35,
        "TLD": "thesportster.com"
      },
      {
        "Frequency": 105,
        "TLD": "kijiji.ca"
      }
    ],
    "updated": 1491970909631
  },
  {
    "BannerCode": 79628,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_BigBox_300x250_SPRINGCLEAN_Apr6_12.6dd2d04ec9eb4cc59a601ccdef51d2b6.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79628_37057_ebay.ca.pdf",
    "TLD": "ebay.ca",
    "_id": "79628_37057_ebay.ca",
    "domains": [
      {
        "Frequency": 865,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 251,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 560,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 298,
        "TLD": "thesportster.com"
      },
      {
        "Frequency": 237,
        "TLD": "thetalko.com"
      }
    ],
    "updated": 1491992484094
  },
  {
    "BannerCode": 79629,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_PLANTER_Apr6_12.5e760f75668a46bca0e03e944c56be93.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79629_37057_mobafire.com.pdf",
    "TLD": "mobafire.com",
    "_id": "79629_37057_mobafire.com",
    "domains": [
      {
        "Frequency": 3,
        "TLD": "mocospace.com"
      },
      {
        "Frequency": 2,
        "TLD": "mobafire.com"
      },
      {
        "Frequency": 16,
        "TLD": "shmoop.com"
      },
      {
        "Frequency": 3,
        "TLD": "easybib.com"
      },
      {
        "Frequency": 4,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491834239538
  },
  {
    "BannerCode": 79629,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_PLANTER_Apr6_12.5e760f75668a46bca0e03e944c56be93.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79629_37057_easybib.com.pdf",
    "TLD": "easybib.com",
    "_id": "79629_37057_easybib.com",
    "domains": [
      {
        "Frequency": 5,
        "TLD": "drudgereport.com"
      },
      {
        "Frequency": 3,
        "TLD": "easybib.com"
      },
      {
        "Frequency": 3,
        "TLD": "mocospace.com"
      },
      {
        "Frequency": 19,
        "TLD": "shmoop.com"
      },
      {
        "Frequency": 10,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491862734677
  },
  {
    "BannerCode": 79664,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TERRA_DblSkyscraper_300x600_EASTER_Apr6_12.743bab0de3ed43329832b3dc94de23bb.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 600,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79664_37057_hockeybuzz.com.pdf",
    "TLD": "hockeybuzz.com",
    "_id": "79664_37057_hockeybuzz.com",
    "domains": [
      {
        "Frequency": 21,
        "TLD": "wikia.com"
      },
      {
        "Frequency": 77,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 56,
        "TLD": "topix.com"
      },
      {
        "Frequency": 47,
        "TLD": "imgur.com"
      },
      {
        "Frequency": 53,
        "TLD": "hockeybuzz.com"
      }
    ],
    "updated": 1491963075321
  },
  {
    "BannerCode": 79630,
    "BannerType": 2,
    "CampCode": 37057,
    "CustomerID": 12175,
    "FileURL": "https://eq-atom.s3.amazonaws.com:443/creatives/12175/TerraEaster_Apr_300x250_70063.9ac1d1fe407b46d582c298452747b65d.jpg",
    "FlightID": 37055,
    "HtmlAd": "",
    "ImgHeight": 250,
    "ImgWidth": 300,
    "OfferID": 37054,
    "ScreenshotURL": "https://eq-atom.s3.amazonaws.com/screenshots/12175/37054/79630_37057_mediatakeout.com.pdf",
    "TLD": "mediatakeout.com",
    "_id": "79630_37057_mediatakeout.com",
    "domains": [
      {
        "Frequency": 65,
        "TLD": "mediatakeout.com"
      },
      {
        "Frequency": 548,
        "TLD": "kijiji.ca"
      },
      {
        "Frequency": 153,
        "TLD": "hockeybuzz.com"
      },
      {
        "Frequency": 557,
        "TLD": "ebay.ca"
      },
      {
        "Frequency": 94,
        "TLD": "addictinggames.com"
      }
    ],
    "updated": 1491938340536
  }
]
```

##### GET `beta/campaigns/37057/stats?dates=2017-04-10,2017-04-11&revenue=true&onlydaily=false&incurrency=true&format=json&user=<USER_EMAIL>&key=<KEY>`

```json
[
  {
    "Revenue": 26.974,
    "clicks": 7,
    "date": "2017-04-10",
    "hour": -1,
    "impressions": 13487
  },
  {
    "Revenue": 0.494,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 8,
    "impressions": 247
  },
  {
    "Revenue": 0.46,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 9,
    "impressions": 230
  },
  {
    "Revenue": 0.368,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 10,
    "impressions": 184
  },
  {
    "Revenue": 0.464,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 11,
    "impressions": 232
  },
  {
    "Revenue": 0.27,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 12,
    "impressions": 135
  },
  {
    "Revenue": 0.488,
    "clicks": 1,
    "date": "2017-04-10",
    "hour": 13,
    "impressions": 244
  },
  {
    "Revenue": 0.772,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 14,
    "impressions": 386
  },
  {
    "Revenue": 0.79,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 15,
    "impressions": 395
  },
  {
    "Revenue": 1.008,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 16,
    "impressions": 504
  },
  {
    "Revenue": 1.036,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 17,
    "impressions": 518
  },
  {
    "Revenue": 0.722,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 18,
    "impressions": 361
  },
  {
    "Revenue": 0.654,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 19,
    "impressions": 327
  },
  {
    "Revenue": 0.304,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 20,
    "impressions": 152
  },
  {
    "Revenue": 0.064,
    "clicks": 0,
    "date": "2017-04-10",
    "hour": 21,
    "impressions": 32
  },
  {
    "Revenue": 6.488,
    "clicks": 4,
    "date": "2017-04-10",
    "hour": 22,
    "impressions": 3244
  },
  {
    "Revenue": 12.592,
    "clicks": 2,
    "date": "2017-04-10",
    "hour": 23,
    "impressions": 6296
  },
  {
    "Revenue": 4.106,
    "clicks": 4,
    "date": "2017-04-11",
    "hour": -1,
    "impressions": 2053
  },
  {
    "Revenue": 0.366,
    "clicks": 1,
    "date": "2017-04-11",
    "hour": 0,
    "impressions": 183
  },
  {
    "Revenue": 0.58,
    "clicks": 1,
    "date": "2017-04-11",
    "hour": 1,
    "impressions": 290
  },
  {
    "Revenue": 0.42,
    "clicks": 0,
    "date": "2017-04-11",
    "hour": 2,
    "impressions": 210
  },
  {
    "Revenue": 0.174,
    "clicks": 0,
    "date": "2017-04-11",
    "hour": 10,
    "impressions": 87
  },
  {
    "Revenue": 0.248,
    "clicks": 0,
    "date": "2017-04-11",
    "hour": 11,
    "impressions": 124
  },
  {
    "Revenue": 1.218,
    "clicks": 2,
    "date": "2017-04-11",
    "hour": 12,
    "impressions": 609
  },
  {
    "Revenue": 0.846,
    "clicks": 0,
    "date": "2017-04-11",
    "hour": 13,
    "impressions": 423
  },
  {
    "Revenue": 0.254,
    "clicks": 0,
    "date": "2017-04-11",
    "hour": 14,
    "impressions": 127
  }
]
```

##### GET `beta/customers/?wlid=51&stats=true&user=<USER_EMAIL>&key=<KEY>`

```json
{
  "ancestor": {
    "HasContract": true,
    "ID": 51,
    "level": "wl",
    "name": "Metroland Digital"
  },
  "customers": [
    {
      "Completed": 3,
      "Currency": "CAD",
      "CustomerID": 12035,
      "CustomerName": "Test Customer",
      "Draft": 3,
      "Paused": 0,
      "Pending": 0,
      "Running": 0,
      "Wallet": null
    },
    {
      "Completed": 0,
      "Currency": "CAD",
      "CustomerID": 12037,
      "CustomerName": "AS Advertising",
      "Draft": 1,
      "Paused": 1,
      "Pending": 0,
      "Running": 0,
      "Wallet": null
    },
    {
      "Completed": 2,
      "Currency": "CAD",
      "CustomerID": 12063,
      "CustomerName": "258984_Lakeridge Chrysler",
      "Draft": 0,
      "Paused": 0,
      "Pending": 0,
      "Running": 0,
      "Wallet": null,
      "delivery": [
        {
          "Actions": 0,
          "Clicks": 0,
          "Date": "2017-03-29",
          "Impressions": 3670,
          "Spend": 14.68
        },
        {
          "Actions": 0,
          "Clicks": 1,
          "Date": "2017-03-30",
          "Impressions": 2949,
          "Spend": 11.796
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-03-31",
          "Impressions": 4375,
          "Spend": 17.5
        },
        {
          "Actions": 0,
          "Clicks": 0,
          "Date": "2017-04-01",
          "Impressions": 4803,
          "Spend": 19.212
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-04-02",
          "Impressions": 4517,
          "Spend": 18.068
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-04-03",
          "Impressions": 4395,
          "Spend": 17.58
        },
        {
          "Actions": 0,
          "Clicks": 5,
          "Date": "2017-04-04",
          "Impressions": 3986,
          "Spend": 15.944
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-04-05",
          "Impressions": 4079,
          "Spend": 16.316
        },
        {
          "Actions": 0,
          "Clicks": 3,
          "Date": "2017-04-06",
          "Impressions": 3949,
          "Spend": 15.796
        },
        {
          "Actions": 0,
          "Clicks": 11,
          "Date": "2017-04-07",
          "Impressions": 9917,
          "Spend": 39.668
        },
        {
          "Actions": 0,
          "Clicks": 19,
          "Date": "2017-04-08",
          "Impressions": 18461,
          "Spend": 73.844
        },
        {
          "Actions": 0,
          "Clicks": 27,
          "Date": "2017-04-09",
          "Impressions": 16648,
          "Spend": 66.592
        }
      ],
      "delivery_avg": {
        "Actions": 0,
        "Clicks": 6,
        "Impressions": 6812,
        "Spend": 27.24966666666666666666666667
      }
    },
    {
      "Completed": 1,
      "Currency": "CAD",
      "CustomerID": 12065,
      "CustomerName": "1442749_Pandora White Oaks Mall",
      "Draft": 0,
      "Paused": 0,
      "Pending": 0,
      "Running": 0,
      "Wallet": null
    },
    {
      "Completed": 1,
      "Currency": "CAD",
      "CustomerID": 12067,
      "CustomerName": "312327_Scarborough Toyota",
      "Draft": 0,
      "Paused": 0,
      "Pending": 0,
      "Running": 0,
      "Wallet": null,
      "delivery": [
        {
          "Actions": 0,
          "Clicks": 5,
          "Date": "2017-03-29",
          "Impressions": 7211,
          "Spend": 14.422
        },
        {
          "Actions": 0,
          "Clicks": 13,
          "Date": "2017-03-30",
          "Impressions": 7372,
          "Spend": 14.744
        },
        {
          "Actions": 0,
          "Clicks": 9,
          "Date": "2017-03-31",
          "Impressions": 7467,
          "Spend": 14.934
        },
        {
          "Actions": 0,
          "Clicks": 0,
          "Date": "2017-04-01",
          "Impressions": 1,
          "Spend": 0.002
        }
      ],
      "delivery_avg": {
        "Actions": 0,
        "Clicks": 6,
        "Impressions": 5512,
        "Spend": 11.0255
      }
    },
    {
      "Completed": 0,
      "Currency": "CAD",
      "CustomerID": 12071,
      "CustomerName": "5198041181_OptiTech Eyewear",
      "Draft": 0,
      "Paused": 0,
      "Pending": 0,
      "Running": 2,
      "Wallet": null,
      "delivery": [
        {
          "Actions": 0,
          "Clicks": 1,
          "Date": "2017-03-29",
          "Impressions": 1178,
          "Spend": 2.356
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-03-30",
          "Impressions": 1193,
          "Spend": 2.386
        },
        {
          "Actions": 0,
          "Clicks": 1,
          "Date": "2017-03-31",
          "Impressions": 1154,
          "Spend": 2.308
        },
        {
          "Actions": 0,
          "Clicks": 0,
          "Date": "2017-04-01",
          "Impressions": 1402,
          "Spend": 2.804
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-04-02",
          "Impressions": 1179,
          "Spend": 2.358
        },
        {
          "Actions": 0,
          "Clicks": 1,
          "Date": "2017-04-03",
          "Impressions": 1176,
          "Spend": 2.352
        },
        {
          "Actions": 0,
          "Clicks": 0,
          "Date": "2017-04-04",
          "Impressions": 1137,
          "Spend": 2.274
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-04-05",
          "Impressions": 1138,
          "Spend": 2.276
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-04-06",
          "Impressions": 1135,
          "Spend": 2.27
        },
        {
          "Actions": 0,
          "Clicks": 2,
          "Date": "2017-04-07",
          "Impressions": 1135,
          "Spend": 2.27
        },
        {
          "Actions": 0,
          "Clicks": 0,
          "Date": "2017-04-08",
          "Impressions": 1136,
          "Spend": 2.272
        },
        {
          "Actions": 0,
          "Clicks": 1,
          "Date": "2017-04-09",
          "Impressions": 1138,
          "Spend": 2.276
        },
        {
          "Actions": 0,
          "Clicks": 0,
          "Date": "2017-04-10",
          "Impressions": 1136,
          "Spend": 2.272
        }
      ],
      "delivery_avg": {
        "Actions": 0,
        "Clicks": 1,
        "Impressions": 1172,
        "Spend": 2.344153846153846153846153846
      }
    },
    {
      "Completed": 0,
      "Currency": "CAD",
      "CustomerID": 12143,
      "CustomerName": "514846_Leons - Peterborough",
      "Draft": 0,
      "Paused": 2,
      "Pending": 0,
      "Running": 0,
      "Wallet": null
    },
    {
      "Completed": 0,
      "Currency": "CAD",
      "CustomerID": 12175,
      "CustomerName": "1477462_Terra Greenhouses ",
      "Draft": 0,
      "Paused": 5,
      "Pending": 1,
      "Running": 3,
      "Wallet": null,
      "delivery": [
        {
          "Actions": 0,
          "Clicks": 10,
          "Date": "2017-04-09",
          "Impressions": 6289,
          "Spend": 12.578
        },
        {
          "Actions": 0,
          "Clicks": 28,
          "Date": "2017-04-10",
          "Impressions": 30100,
          "Spend": 60.2
        }
      ],
      "delivery_avg": {
        "Actions": 0,
        "Clicks": 19,
        "Impressions": 18194,
        "Spend": 36.389
      }
    }
  ]
}
```

##### GET `beta/customers/12035?user=<USER_EMAIL>&key=<KEY>`

```json
{
  "ancestors": [
    {
      "HasContract": true,
      "ID": 51,
      "level": "wl",
      "name": "Metroland Digital"
    }
  ],
  "customer": {
    "Completed": 3,
    "Currency": "CAD",
    "CustomerID": 12035,
    "CustomerName": "Test Customer",
    "Draft": 3,
    "Email": "leo.li@eqworks.com",
    "Paused": 0,
    "Pending": 0,
    "Running": 0,
    "Wallet": null
  }
}
```

##### GET `beta/customers/12035/banners?user=<USER_EMAIL>&key=<KEY>`

```json
[
  {
    "AdvertiserId": 12036,
    "AppNexusAuditResult": null,
    "AppNexusCreativeID": null,
    "BannerCode": 79189,
    "BannerName": "Test 2 creatives",
    "BannerType": 7,
    "Brand": "Test",
    "ExpandDirection": null,
    "ExpandTrigger": null,
    "FileURL": "",
    "FinalUrl": "www.google.com",
    "GoogleAuditResult": null,
    "GoogleCreativeID": "79189 - Test 2 creatives",
    "HtmlAd": "<script type=\"text/javascript\">\ndocument.write('<scr'+'ipt type=\"text/javascript\" charset=\"utf-8\" src=\"http://adserver.adtechus.com/addyn/3.0/5240/3367010/718513/0/loc=100;target=_blank;AdId=9175106;BnId=-1;;misc=' + new Date().getTime() + ';rdclick=\"></scri'+'pt>');\n</script>",
    "ImgHeight": 250,
    "ImgLink": "www.google.com",
    "ImgTarget": "_blank",
    "ImgWidth": 300,
    "IsActive": true,
    "IsExpandable": null,
    "IsPopUnder": null,
    "MaxVideoLength": 0,
    "QSSeparator": null,
    "RMXAuditResult": null,
    "RMXCreativeID": null,
    "RichMediaVendor": null,
    "VastWrapperDepth": null,
    "ZoneCode": 11
  }
]
```

##### GET `beta/customers/12035/banners/79189?user=<USER_EMAIL>&key=<KEY>`

```json
{
  "AdvertiserId": 12036,
  "BannerCode": 79189,
  "BannerName": "Test 2 creatives",
  "BannerType": 7,
  "Brand": "Test",
  "CustomerID": 12035,
  "FileURL": "",
  "FinalUrl": "www.google.com",
  "HtmlAd": "<script type=\"text/javascript\">\ndocument.write('<scr'+'ipt type=\"text/javascript\" charset=\"utf-8\" src=\"http://adserver.adtechus.com/addyn/3.0/5240/3367010/718513/0/loc=100;target=_blank;AdId=9175106;BnId=-1;;misc=' + new Date().getTime() + ';rdclick=\"></scri'+'pt>');\n</script>",
  "ImgHeight": 250,
  "ImgLink": "www.google.com",
  "ImgWidth": 300,
  "ZoneCode": 11
}
```
