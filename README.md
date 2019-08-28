*Note*: Unless otherwise stated, `user` and `key` are essential query parameters for all API endpoints

## API documentations

[Version `beta`](/api_doc_beta.pdf)

## API Sample Responses

### `/beta/campaigns`

##### GET `/beta/campaigns/?cuid=12175&state=running&stats=true&legacy=false&user=<USER_EMAIL>&key=<KEY>`

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
  "campaigns": {
    "37054": {
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
  }
}
```

##### GET `/beta/campaigns/37054?summary=true&incurrency=true&user=<USER_EMAIL>&key=<KEY>`

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

##### GET `/beta/campaigns/37057/banners?cuid=12175&user=<USER_EMAIL>&key=<KEY>`

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
  }
]
```

##### GET `/beta/campaigns/37054/children?level=offer&summary=true&incurrency=true&user=<USER_EMAIL>&key=<KEY>`

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
  }
]
```

##### GET `/beta/campaigns/37057/screenshots?user=<USER_EMAIL>&key=<KEY>`

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
  }
]
```

##### GET `/beta/campaigns/37057/stats?dates=2017-04-10,2017-04-11&revenue=true&onlydaily=false&incurrency=true&format=json&user=<USER_EMAIL>&key=<KEY>`

*Note*: `hour = -1` means the whole day

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
  }
]
```

### `/beta/customers`

##### GET `/beta/customers/?wlid=51&stats=true&user=<USER_EMAIL>&key=<KEY>`

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

##### GET `/beta/customers/12035?user=<USER_EMAIL>&key=<KEY>`

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

##### GET `/beta/customers/12035/banners?user=<USER_EMAIL>&key=<KEY>`

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

##### GET `/beta/customers/12035/banners/79189?user=<USER_EMAIL>&key=<KEY>`

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
