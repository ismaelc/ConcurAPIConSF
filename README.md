<img src="https://jfqcza.bn1.livefilestore.com/y2paqP_3uagi8J3WlP4-pNt4kJoOzRKmuohSQUsrjaegIaoNbNZJ7EXLEflIO6XYAOKM6scpKxbtXPg10RL5OO3A9bc6m-zERVRHUYB1OEGq8s/Concur_Logo_VT_Color_500px.png?psid=1" width="90px" />&nbsp;&nbsp;&nbsp;&nbsp;<a style="text-decoration:none; color:black" name="top" >Concur @ #APIConSF </a> &nbsp;&nbsp;&nbsp;<img src="https://jfqcza.bn1301.livefilestore.com/y2ptjgicP0ebOjYyHeIih7kFg5r2UQWMkL2pdY6M_TPX4tSdTM-NaKW1UF1fiqIdhtiS8mG9uYx1Dzzc-BNKYewC13H-UkBpUx-38WpJITCapA/Screen%20Shot%202014-05-19%20at%203.04.22%20PM.png?psid=1" width="110px" />
=========
<br/>
This page contains information and links to all the resources you need for the **Concur Contest** in #APIConSF Hackathon:

  - [Prize for **Best use of Concur API**](#prizes)
  - [What is Concur?](#concur)
  - [What information can I get from the Concur APIs?](#apis)
  - [I'm sold.. How do I get started?](#getstarted)
  - [Other often-used API calls to check e.g. *POST itinerary information*](#other)
  - [Sample code/libraries](#samplecode)
  - [Help! I'm stuck!](#help)
  - [#APIConSF Sponsor API Links and Prizes](#sponsors)
  - [Mashup with fellow sponsors' APIs](#mashup)

<a name="prizes">Best use of Concur API:</a>
----
        
  - **$500 Amazon gift card**: *Best Use of Concur APIs* - the winning team gets a $500 Amazon gift card.
    

<a name="concur">What is Concur?</a>
-----------

 <img src='https://jfqcza.bn1303.livefilestore.com/y2pDadi2n4fFfdP7nP7r8tv0mYI0vjDmw1VAHp2h7wAz63qmdTheO7CFZNoMHVUM1AYm9-Ur3YHeR8RrN6yJyw0J_UVEqVwCsTqaxqYte1v6Fg/1.png?psid=1' width="200px"/> <img src='https://jfqcza.bn1302.livefilestore.com/y2pbj4PSh8gAbIicwDnrsPoA2qzBF7mZRE9iN6-tiMl7bE0VpuarZE5fGiQJXBPsZ5bLZoK-POwjWMOeTVh5I-2vr9YMxwnN8zjx08fvWHnE04/2.png?psid=1' width="200px" /> <img src='https://jfqcza.bn1301.livefilestore.com/y2pN7PVESkTt9qgjdCJk-aTmoCdKwZ8HonrNlTzylZPrgs_4rWesCjgd9SBV7xAx7BSaQ4c8wwU9GCCplNeGxfqCQPy-2gcw7c6T5n8O-Bm-y4/3.png?psid=1' width="200px" />

**Concur started out as a company that helped business travelers manage their receipts and reimbursements**.  If you've ever filled out an Excel sheet to itemize all your expense items, or carried a separate envelope to make sure you don't lose all your receipts for reimbursement, then you understand the pain that Concur solves for business travelers.  Using software, Concur set out to remove these unnecessary troubles.  

Fast forward to today, through Concur you can **take a picture of your receipts** (and rid yourself of the paper receipt mayhem), **itemize expense** (using OCR and E-Receipts), **submit your expense reports**, and even **book a company policy-compliant travel** (*"Will my boss approve this?"*). This saves companies time and money, and ensures that their business travelers are productive.

Over 25 million people in 190 countries and over 65 percent of the Fortune 500 trust Concur to process $50 billion in travel and expense data per year.  We help these 25M business travelers manage their travel bookings and expense reports through the Concur Travel and Expense web/mobile app. 

With this global reach, we have opened up the [Concur Platform](http://developer.concur.com/) so that partners can provide value to Concur users by having access to their itinerary and expense information.    

**That's where you come in**.

<a name="apis">What information can I get from the Concur APIs?</a>
--------------

**Example apps**

Let's first look at 2 examples of apps that our partners have built using Concur APIs.  They're all listed in our [App Center](https://www.concur.com/en-us/app-center):

- [TravelText](https://www.concur.com/en-us/partners/transaction-capture/traveltext) - TravelText allows you to text your expenses right into Concur. No more paper receipts and Excel sheet mayhem!  Don't believe us?  Check out their video demo [here](https://www.youtube.com/watch?v=sxY_PO-QKZ0).

- [Trover](https://www.concur.com/en-us/app-center/listing/nDhf34TiiC9RCocFM2xViin5c/Trover) - it's travel photography + business travel integration in one great app. Because we understand that the business traveler is a person too. Quoting from this [article](http://skift.com/2013/07/25/travel-photography-app-trover-secures-2-5-million-in-funding-from-concur/#/0), what they get for integrating with Concur is *"being able to tap into Concur’s experience, knowledge and “great visibility into travel patterns”"*.

**Information returned by the APIs**

You can find more examples of apps that use our APIs in the App Center link above.  Now let's get to business - what information can you get from the Concur APIs?
- [Expense data history of a Concur user](https://developer.concur.com/api-documentation/web-services/expense-report/expense-report-resource/get-report-digests) - users of Concur expense their purchases using the Concur Travel and Expense web/mobile app, so that they can get reimbursed by their company at the end of the trip.  This gives Concur insight into a user's expense pattern (*e.g. does Joe always get a Starbucks coffee right after landing in SFO?*). This API returns a collection of expense reports that you can use to make the same deduction.  It's also worth noting that there are also APIs to submit expense [entries](https://www.concursolutions.com/api/docs/index.html#!/Entries/Post_content_user_post_2) (e.g. Starbucks coffee, printer ink, etc) and [reports](https://developer.concur.com/api-documentation/web-services/expense-report) (collection of expense entries), as well as [submit images](https://www.concursolutions.com/api/docs/index.html#!/ReceiptImages) of receipts (similar to TravelText above).
                                                                                        
- [Itinerary Details of a Concur user](https://developer.concur.com/api-documentation/web-services/itinerary/itinerary-resource/itinerary-resource-get#getitindetails) - there's a ton of information you can get from a Concur user's trip, such as the booking segments the trip, whether it's Air, Car, Hotel, Dining, Ride, Rail, or Parking.  The most common information you'll probably use is a user's travel destination.  From that single piece of info, you can make recommendations to the travele (just like Trover).

These are just two of [many APIs](http://developer.concur.com/) you can use to get information from Concur.

<a name="getstarted">I'm sold, how do I get started?</a>
----

**Quickest Way (5 mins) - a GET API call**
--

To save you time, we have created developer test accounts pre-populated with expense and itinerary information.  The idea is to quickly familiarize you with the structure of expense and itinerary information that you can get from Concur.  We still expect you to understand the normal flow from a Concur user's perspective, which is why we will explain that bit later.  For now, all you need is an access token, and call an API, the Expense Report Digest API in this case, like this:

        curl https://www.concursolutions.com/api/v3.0/expense/reportdigests
        -H "Authorization: OAuth <insert your access token here>"

A similar call to get an Itinerary List of a Concur user would be:

        curl https://www.concursolutions.com/api/travel/trip/v1.1
        -H "Authorization: OAuth <insert your access token here>"

**To get a JSON response**, you can do a GET call like below:

        curl https://www.concursolutions.com/api/v3.0/expense/reportdigests
        -H "Authorization: OAuth <insert your access token here>"   
        -H "Accept: application/json"
        
**To POST JSON content**, add the following header:

        -H "Content-Type:application/json"

To get an access token, send an email to chris.ismael@concur.com (our Developer Evangelist) or approach him at the Concur booth and say "Gimme!"

You can also give our [Swagger API documentation](https://www.concursolutions.com/api/docs/index.html) a spin.  We'll cover Swagger in a bit more detail below.

**Normal Way - Generate an access token and use the Concur mobile app**
--

The section explains how to properly authenticate against the Concur APIs by generating your own access token, and using the Concur app to create an Expense Report.  The last step would be to call the Entries API to pull the individual line items inside the Expense Report we created.  To get started, first we need to get a developer sandbox account, and install the Concur app.

**Get a Developer sandbox account**

A developer sandbox account allows you to test both the app and APIs, free of charge.  For the purposes of this hackathon, we have set up developer accounts (using non-existent email addresses and pre-populated with Expense and Itinerary information) so that you can start using them right away.  To get one of these accounts, please email chris.ismael@concur.com with the Subject: Concur Sandbox Request.  

If you prefer to set up your own free sandbox, you can do so by registering [here](https://developer.concur.com/register).  Note that the setup steps right after you login requires you to keep clicking 'Next' (for the most part) until you get to the end.  If you get stuck, reach out to chris.ismael@concur.com or send him a tweet @chrispogeek

**Install the app**

After you've set up your sandbox account, start familiarizing yourself with the app, so that you can map the APIs to features inside the product.  You can access the web version of Concur at http://concursolutions.com/ or get the mobile app from [App Store](https://itunes.apple.com/us/app/concur-travel-receipts-expense/id335023774?mt=8) or [Google Play](https://play.google.com/store/apps/details?id=com.concur.breeze).

It helps to watch these [2-min videos](https://www.concur.com/en-us/resource-center/mobile?type[]=video) (snapshot image below) to understand how the Concur app works, as well as get context on how your app will add value to the Concur business traveler (e.g. Our app helps Concur users predict weather conditions for their future travel).

<img src='https://jfqcza.bn1301.livefilestore.com/y2plGwIFgIkWPhuXtK609Lokwso2nQKF5qZjZa0lQZI8p2WZl2s2s2VrbHQhyOVE8nJZm1iVnjxfqC4pH_CXEKxiSMcNl_LF2iXW10hfM3YGPk/Screen%20Shot%202014-04-22%20at%2010.37.30%20PM.png?psid=1' width="600px" />

**Generate Access Token -> Create Expense Report in App -> Call API**

The steps below show how we can generate an access token for the API call, use the Concur app to create an Expense report, and getting back individual items inside that expense report through an API call.  Without getting into too much detail, we'll authenticate using Concur's [OAuth Native Flow](https://developer.concur.com/api-documentation/oauth-20-0#nativeexample).  The goal is to get an Access Token that we will use for all our subsequent API calls. (*Note: You can also use the [OAuth Web Flow](https://developer.concur.com/api-documentation/oauth-20-0#webstep) that shows a Concur login page to collect the user's credentials*)

1.   **Get your Consumer Key**  

 After logging in to http://concursolutions.com, go to Administration -> Register Partner Application -> Concur Partner Application (Modify).  We need the consumer key so we can call the endpoint that would return the access token.

 <img src='http://chrispogeek.files.wordpress.com/2014/01/untitled.png' width="600px" />

2.  **Call the endpoint to request an access token**

 Here's what the HTTP call looks like to request for an access token:

        GET https://www.concursolutions.com/net2/oauth2/accesstoken.ashx HTTP 1.1
        Authorization: Basic am9obl9kZXZlbG90bWFpbC5jb206VHJhdmVsJkV4cGVuc2UkMjAxMg==
        X-ConsumerKey: eZByXv2X41cJlC21pSVvRi    

 Note that we already have `X-ConsumerKey` from number 1.  To generate the `Authorization: Basic` value, you need to Base64-encode the login ID, colon and password such that john_developer@hotmail.com:Travel&Expense$2012 becomes am9obl9kZXZlbG90bWFpbC5jb206VHJhdmVsJkV4cGVuc2UkMjAxMg==.  If you're not doing this programmatically yet, you can use this [nifty web tool](http://www.base64encode.org/) to generate that value (remember to choose Encode).

 If you're using a Terminal, an equivalent curl statement of the above would be:
        
        curl https://www.concursolutions.com/net2/oauth2/accesstoken.ashx
        -H "Authorization: Basic am9obl9kZXZlbG90bWFpbC5jb206VHJhdmVsJkV4cGVuc2UkMjAxMg=="
        -H "X-ConsumerKey: eZByXv2X41cJlC21pSVvRi"

 If the call is successful, you should get an XML response with a `<Token>` node.  That's your access token. We would also recommend that you use [Postman](http://www.getpostman.com/), a Chrome extension, to help you manage your API calls (not just Concur ones).  Here's what it looks like in action:

 <img src='http://chrispogeek.files.wordpress.com/2014/01/screen-shot-2014-01-13-at-4-45-35-pm.png' width="600px" />

 *Chris has already built a couple of Concur Postman "Collections", email him at chris.ismael@concur.com if you want to get it.*

3.  **Create items to expense and associate them with an expense report**

 We will do this bit using the Concur mobile app.  This would give us data that we can pull using the APIs.  Note that aside from Expense, we can do the same thing for Travel too.  Here's a sequence of screenshots on how to add an expense using the app, then associating them with an expense report.

 <img src='https://jfqcza.bn1303.livefilestore.com/y2pDadi2n4fFfdP7nP7r8tv0mYI0vjDmw1VAHp2h7wAz63qmdTheO7CFZNoMHVUM1AYm9-Ur3YHeR8RrN6yJyw0J_UVEqVwCsTqaxqYte1v6Fg/1.png?psid=1' width="200px"/> <img src='https://jfqcza.bn1302.livefilestore.com/y2pbj4PSh8gAbIicwDnrsPoA2qzBF7mZRE9iN6-tiMl7bE0VpuarZE5fGiQJXBPsZ5bLZoK-POwjWMOeTVh5I-2vr9YMxwnN8zjx08fvWHnE04/2.png?psid=1' width="200px" /> <img src='https://jfqcza.bn1301.livefilestore.com/y2pN7PVESkTt9qgjdCJk-aTmoCdKwZ8HonrNlTzylZPrgs_4rWesCjgd9SBV7xAx7BSaQ4c8wwU9GCCplNeGxfqCQPy-2gcw7c6T5n8O-Bm-y4/3.png?psid=1' width="200px" />
 
 You can keep adding new expenses (and even add a receipt image!) to have a variety of data to pull for your API calls.  After adding expenses, create a report to associate it with by tapping the "Add to Report" button (in the last screenshot above).

4.  **Call the APIs to pull expense report items**

 Since we now have an access token, we can pull an Expense Report Digest, like so (in Terminal):

        curl https://www.concursolutions.com/api/v3.0/expense/reportdigests
        -H "Authorization: OAuth <insert your access token here>"
 
 This would return an Expense Report response, with a field called `ID`.  We need this ID to extract the expense line items we created in the app earlier.  To liven things up a bit, let's use the [Swagger](https://www.concursolutions.com/api/docs/index.html#!/Entries) documentation of the "Entries" API to get the individual expense line items:

 <img src='https://jfqcza.bn1302.livefilestore.com/y2pExFhXefF7BWcggCWbeRkUyOUyEf1UdRi0HoCcpj8PKfaGMub-K8xc0BXHsX2NUFlNp54-m6X3aJ7dRNLQiIHfyYJhdtTiEJEArnZJ-r7NCA/Screen%20Shot%202014-04-22%20at%201.21.55%20PM.png?psid=1' width="600px" />

 We highlighted two things here, the (oval) field where you put in your access token, and the (rectangle) field where you put in the `ID` we got from the previous API call.  Note that we can do this same call in curl, or in any fashion you want.  Swagger just provides us a consolidated way to make the API calls.

 To execute the call, click the "Try it out!" button.  You should get a response like this below:

 <img src='https://jfqcza.bn1304.livefilestore.com/y2pty6lMBv5XXLjA_mT5HLpSNea4hVr3AUCRuEI207Wr1otLVxy86klHYuNDP0N-cvb75IFJvicR1jR2K7X3wqJXsH_AQNcEWkp6iO4t3jXRCs/Screen%20Shot%202014-04-22%20at%201.29.22%20PM.png?psid=1' width="600px" />

[Back to Top](#top)

<a name="other">Often-used API calls/samples:</a>
--

**How to make a POST call to create an itinerary:**

Here are details of an HTTP POST call push itinerary to a Concur user's trip list:

     Request Type = POST
     Authorization = <your access token>
     URI = https://www.concursolutions.com/api/travel/trip/v1.1/
     ContentType = Application/XML
     Body = 
      <?xml version="1.0"?>
      <Itinerary xmlns="http://www.concursolutions.com/api/travel/trip/2010/06">
      <TripName>TechCrunch Disrupt Concur</TripName>
      <StartDateLocal>2014-05-30T03:47:14</StartDateLocal>
      <EndDateLocal>2014-06-06T03:47:14</EndDateLocal>
      <Bookings>
       <Booking>
        <Segments>
            <Hotel>
                <Status>HK</Status>
                <StartCityCode>SFO</StartCityCode>
                <StartDateLocal>2014-05-30T07:47:14</StartDateLocal>
                <EndDateLocal>2014-06-06T03:47:14</EndDateLocal>
                <Name>Times Square Hilton New York</Name>
                <RecordLocator>Hotel Locator</RecordLocator>
                <RoomDescription>1 KING BED ACCESSIBLE ROOM - K1RRC</RoomDescription>
                <Currency>USD</Currency>
                <CancellationPolicy>Cxl 1 day prior to Arrival</CancellationPolicy>
                <DailyRate>240.3500</DailyRate>
                <NumRooms>1</NumRooms>
                <NumPersons>1</NumPersons>
                <RateCode>LV4</RateCode>
                <Charges>
                    <Rate>
                        <Currency>USD</Currency>
                        <Amount>10.00</Amount>
                        <StartDatelocal>2014-05-30T07:47:14</StartDatelocal>
                        <IsPrimary>false</IsPrimary>
                        <SemanticsCode>ROOMRATE</SemanticsCode>
                        <PerUnit>DAY</PerUnit>
                        <NumUnits>3.00</NumUnits>
                    </Rate>
                </Charges>
            </Hotel>
        </Segments>
        <RecordLocator>Disrupt123</RecordLocator>
        <BookingSource>Sample Itin for Disrupt</BookingSource>
        <DateBookedLocal>2014-04-30T03:47:14</DateBookedLocal>
      </Booking>
      <Booking>
        <Segments>
            <Air>
                <Vendor>AA</Vendor>
                <FlightNumber>425</FlightNumber>
                <StartCityCode>SFO</StartCityCode>
                <StartDateLocal>2014-05-30T03:47:14</StartDateLocal>
                <EndCityCode>NYC</EndCityCode>
                <EndDateLocal>2014-05-30T07:47:14</EndDateLocal>
                <Cabin>O</Cabin>
                <ClassOfService>O</ClassOfService>
            </Air>
        </Segments>
        <RecordLocator>Air Locator</RecordLocator>
        <BookingSource>Sample Itin for Disrupt</BookingSource>
        <DateBookedLocal>2014-04-30T03:47:14</DateBookedLocal>
      </Booking>
    </Bookings>
    </Itinerary>
    
**How to submit an image receipt to Concur (PHP/curl):**

    <?php
        // Please refer to 
        // https://www.concursolutions.com/api/docs/index.html..
        // #!/ReceiptImages/Post_loginID_post_2
        // For instructions to generate access token, please refer to 
        // https://developer.concur.com/api-documentation/oauth-20-0#nativeexample

        $url = "https://www.concursolutions.com/api/v3.0/expense/receiptimages";

        $ch = curl_init();
        
        curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
        curl_setopt($ch, CURLOPT_VERBOSE, 1);
        
        curl_setopt($ch, CURLOPT_URL, $url);
        curl_setopt($ch, CURLOPT_POST, 1);
        curl_setopt($ch, CURLOPT_POSTFIELDS, file_get_contents('./tmp/image.jpg'));
        curl_setopt($ch, CURLOPT_HTTPHEADER, array(
                'Authorization: OAuth <YOUR ACCESS TOKEN HERE>',
                'Content-Type: image/jpeg'
        ));

        $response = curl_exec($ch);
        curl_close($ch);

        echo $response;

    ?>
    
**Posting Report Header:**

    Request Type = POST
    Authorization = <your access token>
    URI = https://www.concursolutions.com/api/expense/expensereport/v1.1/report
    ContentType = Application/XML
    Body = 
    <Report xmlns="http://www.concursolutions.com/api/expense/expensereport/2011/03">
        <Name>Disrupt Hackathon NYC Trip</Name>
        <Purpose>All Hackathon Expenses</Purpose>
        <Comment>Includes hotel and meals.</Comment>
        <OrgUnit1>US</OrgUnit1>
        <OrgUnit3>Bellevue</OrgUnit3>
        <Custom1>Client</Custom1>
        <Custom2>Local</Custom2>
        <UserDefinedDate>2014-05-01 15:15:07.0</UserDefinedDate>
    </Report>

**Getting Report Details:**

    Request Type = GET
    Authorization = <your access token>
    URI = https://www.concursolutions.com/api/expense/expensereport/v2.0/Reports/?reportcountry=US
    ContentType = Application/JSON

**Posting Report Entry:**

    Request Type = POST
    Authorization = <your access token>
    URI = https://www.concursolutions.com/api/expense/expensereport/v1.1/report/B6F4FD62FB424911A3B8/entry
    ContentType = Application/XML
    Body = 
    <ReportEntries xmlns="http://www.concursolutions.com/api/expense/expensereport/2011/03">
    <Expense>
        <CrnCode>USD</CrnCode>
        <ExpKey>BRKFT</ExpKey>
        <Description>Starbucks for Breakfast</Description>
        <TransactionDate>2014-05-01</TransactionDate>
        <TransactionAmount>15.54</TransactionAmount>
        <Comment>Breakfast meeting</Comment>
        <VendorDescription>Starbucks</VendorDescription>
        <IsPersonal>N</IsPersonal>
    </Expense>
    </ReportEntries>

[Back to Top](#top)

<a name="samplecode">Sample code</a>
--------------
- [Windows 8 C#/XAML](https://github.com/ismaelc/Concur-Windows8-SampleCode)
- [Objective-C/iOS](https://github.com/concurtech/mobile-samples)
- [C#](https://github.com/concurtech/api-samples)
- [PHP/curl](http://runnable.com/UtWlKVi9ZnsnAABx/upload-receipts-to-concur-using-php-curl) (in Runnable.com)
- [Python](https://gist.github.com/Trudeaucj/09c25e79c332e93703a0) (Generate access token)
- [node.js](https://github.com/sckuo/node-concur)

[Back to Top](#top)

<a name="help">Help! I'm stuck!</a>
--
 - How do I GET/POST JSON?
 
   **To get a JSON response**, you can do a GET call like below:

        curl https://www.concursolutions.com/api/v3.0/expense/reportdigests
        -H "Authorization: OAuth <insert your access token here>"   
        -H "Accept: application/json"
        
   **To POST JSON content**, add the following header:

        -H "Content-Type:application/json"

 - If you're getting an error when submitting an expense report, it's likely because you have not set up an Account Code for an expense item type (i.e. Account Code `111` for the `Breakfast` type).  To fix this, go to **Setup -> Expense -> 4)Expense -> Expense Types -> 2) Account Code** (as in the screenshot below), and fill out account codes for expense types you're using.  Remember to hit the Save button (right beside the drop-down with the value DEFAULT).
 
 <img src="https://jfqcza.bn1303.livefilestore.com/y2pP9WXkTCzHaovVGVCj0p4K2D3Z2mVS2H6doVFHOS6NXp86kiKYK-upPireIAt7UMR-7zWXoyuYDGV2IJ2d4-HsYFZ1elTzJn3XDzwvXiDxuA/Screen%20Shot%202014-05-01%20at%206.02.26%20PM.png?psid=1" width="600px" />

 - Still stuck? Send Chris an email at chris.ismael@concur.com or tweet @chrispogeek and he'll come to your rescue

[Back to Top](#top)

<a name="mashup">Mash-up with fellow sponsors' APIs</a>
--
Hit more birds with 1 stone with these Concur integration ideas.

Mashup | Idea
------------- | -------------
Concur + Evernote | Auto-upload receipt images dropped in an [Evernote](http://dev.evernote.com/) folder
Concur + Getty Images | Create a [Getty](http://api.gettyimages.com/) photo/video collage of a traveler's itinerary (search images for "Hotel Fairmont San Francisco") to familiarize him/her with the location prior to arrival
Concur + Nexmo | Auto-share your [Nexmo](https://www.nexmo.com/) number to colleagues based on destination country (from Concur).  At the end of your business trip, automatically send your boss an email on how much money you saved the company by accepting SMS/calls through your Nexmo number.
Concur + Twitter | No time for leisure travel on a business trip? [Tweet](https://dev.twitter.com/) random images of places you will never go to, based on your Concur travel destination. Personalize your tweets by pulling Concur expense history (e.g. "Machiatto! [Pic] You all know I heart coffee!"). *This idea was inspired by "Wisconsin" in TechCrunch Disrupt NY Hackathon 2014*
Concur + Pubnub | Build a Swarm clone for business travelers! [Biz Swarm]((http://www.pubnub.com/developers/))! *tagish!*
Concur + Eagle Eye Networks | Take [selfies](http://www.eagleeyenetworks.com/support/api-docs/) at various locations in a hotel (Need help here?)
Concur + Mojio | Compute and submit car mileage expense 
Concur + Orchestrate | Add rich [Orchestrate](https://orchestrate.io/docs/api/) meta-data to a Concur user
s travel and expense for interesting data analysis (e.g. Add restaurant POIs to a Concur user's T&E data to identify opportunities and trends - he could have saved $35 on coffee if he just walked around the block) 
Concur + Wit.ai | Hold up a receipt to your phone camera and [say the total](https://wit.ai/docs/quickstart) so that it gets sent directly to your Concur expense
Concur + SecureKey | Tighten your own Concur Expense/Travel app with [Securekey](http://developer.securekey.com/development/api-guides/)

[Back to Top](#top)

<a name="sponsors">#APIConSF Sponsor API Links and Prizes</a>
--

Sponsor  | Prizes
------------- | -------------
[Concur Technologies](http://bit.ly/ConcurDisrupt)   | $500 Amazon gift card to winning team
[Evernote](http://dev.evernote.com/) | (1) iPad per team member
[Getty Images](http://api.gettyimages.com/) | $1,000 to one team
[Nexmo](https://www.nexmo.com/) | (1) Mini Jambox per team member
[Twitter](https://dev.twitter.com/) | To be announced
[PubNub](http://www.pubnub.com/developers/) | To be announced
[Eagle Eye Networks](http://www.eagleeyenetworks.com/support/api-docs/) | $1,000 cash to one team
[Mojio](https://sandbox.developer.moj.io/) | To be announced
[Orchestrate](https://orchestrate.io/docs/api/) | 1 year subscription to Orchestrate database per team member
[Wit.ai](https://wit.ai/docs/quickstart) | To be announced
[SecureKey](http://developer.securekey.com/development/api-guides/) | 1st place: $1000 AMEX Gift Card, 2nd place: $600 AMEX Gift Card, 3rd place: $400 AMEX Gift Card + all winning teams receive 1 year license of briidge.net CONNECT ID Digital Service

[Back to Top](#top)



**You're set.  Go win this!**
