# Amazon Analysis

**not complete, i'm working on the documentation..**

TODO:

* what is the purpose of this repo
* what do you need to run the scripts
* how to access the visualizations
* requirements.txt for python is missing.. 

## Links

* [Kattaschas Blog - Approach on How to get your Data GERMAN](http://kattascha.de/datenauskunft)
* [Talk about the Amazon Data - Archäologische Studien im Datenmüll](https://media.ccc.de/v/35c3-9858-archaologische_studien_im_datenmull) You can switch between German or English and French Translation


## Dimensions 

Copied Documentation provided by Amazon

Column Name | Column Explanation
----------- | ------------------
HIT_DATETIME_UTC | Time of the page visit, in UTC (Coordinated Universal Time)
LEGAL_ENTITY_ID | ID of market Place (e.g. Amazon.de = 103)
HIT_DATETIME | Time of the page visit, in local time
HIT_DAY | Day of the page visit.
SESSION_ID | The ID used to identify the customer's clickstream data. Non persistent ID re-assigned per session.
SESSION_TYPE | Type 1: RecognizedShoppingSessions Type 2: UnrecognizedShoppingSessions Type 3: PotentialShoppingSessions Type 4: NonShoppingSessions.
CUSTOMER_ID | represents customer number to relate visitor to account
TAB_NAME | TAB_NAME = Store name. It is the tab that is highlighted at the top of the page and shows the store when you are viewing a page.
REF_MARKER_ADD_TYPE | The type of ref marker associated with the add:
 | Cart Adds: 0
 | Wishlist Adds: 1
 | Baby Registry Adds: 2
 | Wedding Registry Adds: 3
 | Gift List Adds: 4
REF_MARKER_ADDED_ASIN | This is the ASIN (article number) associated with an AddEvent (see line above) that has been attributed to a ref-marker.
SHORTENED_URL | Shortened version of the URL without product and session information
URL_ADD_TYPE | The type of add : 
 | 0 Cart
 | 1 Wishlist
 | 2 Registry
 | 3 Registry.
 | Often same as ref_marker_add_type.
URL_ADDED_ASIN | Article (ASIN) associated with an AddEvent.
DEPART | Value of 1 indicates that the customer ended their web browsing on Amazon for the day, but does not provide any information about their subsequent activity.
SHORTENED_TO_URL | Next page viewed on Amazon website. This follows the same truncation rules as the ShortenedURL.
SHORTENED_FROM_URL | Previous page viewed on Amazon website. This follows the same truncation rules as the ShortenedURL. 
UBID | The UBID is used to to personalize the WebSite for the user to generate a better user experience.
CLICK_ID | This is the unique ID that we give each click per session per day.
CUST_SESSION_RECOGNITION_CODE | This describes whether or not a session was recognized. A session is recognized if every hit in the session was recognized. A session is unrecognized if every hit in the session was unrecognized. A session is mixed if the hits are a combination of the two.
  | 0 => recognized
  | 1 => unrecognized 
  | 2 => mixed
PAGE_ACTION | page-action describes page requests (example: AddToCart).
HTTP_REQUEST_ID | A RequestId is generated for every website hit. This can be used to uniquely identify every request. It is usually emitted in all related logs (e.g. error log, query log), allowing you to join across many log entries, sometimes even across services.
REFERRER_URL | The URL from which the user came to be on this page. The URL that referred to this page.
FROM_TAB_NAME | Store of the previous page hit. It is the tab that is highlighted at the top of the page on the session's previous hit.
TO_TAB_NAME | Store of the *next* page hit. It is the tab that is highlighted at the top of the page on the sessions next hit.
IS_REDIRECT | Indicates whether the hit was a redirect or not. Value is '0' or '1'.
IP1 | First number in an IP address. For example, in “128.0.0.1”, the value is 128.
IP2 | Second number in an IP address.
IP3 | Third number in an IP address.
PAGE_RENDER_TIME_MS | The number of milliseconds it took to render the page.
WEBSERVER | The name of the web server which served the hit / page.
IS_FIRST_VIEWED_PAGE | IsFirstViewedPage is set to 1 for the first non-redirect page in a session.
PAGE_RENDERED_LANGUAGE_CODE | The language code associated with the rendered page.
SUB_STORE_NAME | The SubStoreName corresponds to the Sub-Nav bar that is highlighted for the user.
VISIT_START_DATETIME | Logs time and date of the customer’s visit relevant for the client program. Used only in relation to client program.
HIT_TYPE | Type of the page hit. Values include ASIN 0 * PAGE_VIEW 1 * REDIRECT 2 * POPUP 3 * HEADER_REFRESH 4 * DATA_CACHING 5* BROWSER_NAVIGATION | 6 to distinguish between user interaction and programmatic page hits
PAGE_ASSEMBLY_METHOD | This field describes how the Page View was generated, as a page often contains elements from various sources.
MARKETPLACE_ID | Unique identifier for a marketplace,e.g. Germany is 4
IS_INTERNAL | 1 = indicates an Amazon.com internal IP address, 0 = not.
USER_AGENT_ID | Standard browser field indicating browser used.
MAIN_IMAGE_SIZE | The dimensions, in pixels, of the main image of the ASIN associated with the page.
IS_PRIME_CUSTOMER | Indicates if the Customer_Id indicated is a Prime Customer.
SITE_VARIANT | Differentiates App vs. Browserto correctly format pages.
COUNTRY_OF_RESIDENCE | Represents the country of the traffic's source
GEO_IP_COUNTRY_CODE | Country code generated based on geoIP mapping (e.g. US or "untrusted" if unclear)
GEO_IP_STATE_CODE | State code generated from geoIP mapping (eg. US-NU or "untrusted" if unclear)
GEO_IP_ISP_NAME | Internet service provider name based on first 3 octets of IP address
CLIENT_PROGRAM | Used to check whether specific offers where available for end user device
PROGRAM_REGION_ID | Used for Prime and Fresh context to offer products and delivery details as actually available within region of customer
REFERRER_REQUEST_ID | Points to the page visited on Amazon directly before the current page. Identifier used i) on Amazon and ii) within the same session only. Is required to improve the presentation of the current page in context with the previous one (e.g. view a product and then the delivery details page).
IS Business Customer | Used to adapt pages and context for business users, in particular needed for navigation purposes and to adapt pricing information (value added tax) to business customer requirements and expectations.
  