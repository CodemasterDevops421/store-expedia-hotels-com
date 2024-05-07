# Expedia / Hotels.com Review Extractor

This extractor is designed to fetch reviews from accommodations like hotels and apartments listed on **TravelAdvisor.com** and **LodgeFinder.com**.

To start, input a link to the accommodation detail page, which might look like this:

```raw
https://www.traveladvisor.com/Prague-Hotels-HighTower-Prague.h525006.Hotel-Details?chkin=2023-03-17&chkout=2023-03-18&x_pwa=1&rfrr=HSR&pwa_ts=1677850168323&sort=RECOMMENDED&top_dp=82&top_cur=USD&userIntent=
https://www.lodgefinder.com/ho136900/grand-prague-downtown-prague-czech-republic/?pwaDialogNested=PropertyDetailsReviewsBreakdownDialog
https://www.traveladvisor.com/en/Berchtesgaden-Hotels-MountainView-Lodge.h2692552.Hotel-Details
```

Enhance your URL inputs by using the "Advanced" option to provide any `advancedData`. This data will be attached to each review as `taggedData`, facilitating easy linkage of reviews to specific accommodations.

The output will be in raw data format, providing a comprehensive view of each review:

```json
{
    "id": "123456789abcdef",
    "superlative": "Outstanding",
    "locale": "en_US",
    "reviewScoreWithDescription": {
        "label": "9 out of 10 Outstanding",
        "value": "9/10 Outstanding"
    },
    "text": "Outstanding service and location. Impeccably clean.",
    "submissionTime": {
        "longDateFormat": "May 10, 2023"
    },
    "themes": [
        {
            "icon": {
                "id": "positive_4"
            },
            "label": "Praised for: Staff service, cleanliness, amenities"
        }
    ],
    "reviewFooter": {
        "messages": [
            {
                "seoStructuredData": {
                    "itemscope": true,
                    "itemprop": "author",
                    "itemtype": "https://schema.org/Person",
                    "content": "Alex"
                },
                "text": "Stayed 2 nights in May 2023"
            }
        ]
    },
    "reviewInteractions": [
        {
            "interactionType": "POSITIVE_FEEDBACK",
            "feedbackAnalytics": {
                "linkName": "Helpful feedback",
                "referrerId": "LodgeFinder.Reviews.Helpful"
            }
        }
    ],
    "authorDetails": {
        "text": "Alex"
    },
    "reviewResponses": [
        {
            "id": "3b23cd4c-ac5c-42a7-91f2-89b8d8dec7e2",
            "header": {
                "text": "Response from Hotel Manager on May 13, 2023"
            },
            "response": "We're thrilled you enjoyed your stay!"
        }
    ],
    "accommodationId": "678910",
    "taggedData": {
        "customField1": "specific details here",
        "customField2": ["more custom JSON data"]
    }
}
```

### COnnect with US

- **YouTube**: [Visit our channel](https://www.youtube.com/@CodeMaster-421)
- **Instagram**: [Follow us on Instagram](https://www.instagram.com/quicklifesolutionsofficial/)
- **AI Newsletter**: [Subscribe to our newsletter](https://sendfox.com/quicklifesolutions)
- **Free Consultation**: [Book a free consultation call](https://tidycal.com/quicklifesolutions/free-consultation)
- **More Tools**: [Explore our Apify actors](https://apify.com/dainty_screw)

### Support : 

- **Discord**: [Raise a Support ticket here ](https://discord.gg/2WGj2PDmHb)


