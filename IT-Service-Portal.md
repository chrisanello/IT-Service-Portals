#
# Lab Guide

# Service Portal:

# Building Effective IT Service Portals

#
### Chris Anello  &amp; Leonardo Ferreira

Default Login / Password:

admin / knowledge18

abel.tuter / knowledge18

aileen.mottern / knowledge18

###

###

###





## This

## Page

## Intentionally

## Left

## Blank

## User Personas

| **Avatar** | **User** | **Role** | **Expectations** |
| --- | --- | --- | --- |
|   | System Administrator | Service Portal Admin | This person is tasked to create the new Lightspeed Enterprise IT Service Portal. He is not a web developer but has a basic understanding of the web tech concepts. |
|   | Abel Tuter | Employee | Abel is a user of the IT Service Portal. He wants to order new IT Assets, ask questions or just check the Knowledge Base. |
|   | Aileen Mottern | Manager | Aileen is also a user of the IT Service Portal. But as a manager of Abel she also wants to approve the items Abel requested through the Service Portal |

## Lab Files

The following files are need to complete this lab; you can download them via the following links:

| **Picture** | **Name** | **Download Link** |
| --- | --- | --- |
|   | logo.png | [https://goo.gl/gKxJcg](https://goo.gl/gKxJcg) |
|   | background.png | [https://goo.gl/gKxJcg](https://goo.gl/gKxJcg) |

## Lab 1.0 Getting Faimiliar with Servie Portal

## Lab Goal

Welcome to the Service Portal lab! This lab familiarizes you with the default Service Portal.

The Service Portal is a powerful framework used to rapidly build rich web applications using modern web design concepts for the ultimate User Experience. Take a few moments to get familiar with the default portal.

# Browse the Service Portal

1. Browse to your instance and add suffix **/sp**
Log in as **Abel Tuter** , using the credentials provided on cover.
https://&lt;your instance&gt;.service-now.com/sp
2. The default Service Portal should look like the example.


3. Take a few minutes to discover the Service Portal. Go over the different items (Knowledge Base, Get Help, Community).
4. From the homepage; navigate to **Order Something**.
Select a category of your preference, for example **Hardware**.
Select the item you want to order.
When ordering an item; please note the option **Add to Cart**. This gives the user the online web shop experience.
5. Once you added some items to your cart, click the cart icon  in the menu bar.
Select **View Cart**.
6. Here users can still adjust their selection. Click the button **Checkout**.
7. A new request item (REQxxxxxx) is created. Later in this lab, you use a widget to present the user with a list of his/her requested items.
8. Lab 2.0
Create Your Own Portal

## Lab 2.0 Create your Own Portal

## Lab Goal

Your company, **Lightspeed Enterprise** , took the strategic initiative to improve the IT Service Portal Experience. You, as the ServiceNow Administrator, are tasked with designing the new experience where your users can request new mobile work devices such as laptops and tablets. This lab explains how to:

- Create a new, empty Service Portal from scratch
- Apply some basic branding to your portal

# Create the Portal

1. Go to your instance (without the **/sp** suffix).
https://&lt;your instance&gt;.service-now.com/
Your browser might remember the credentials of Abel from Lab 1; first, logout.


2. Log in with the admin credentials.


3. Before creating your own portal, clone the default landing page (index). You&#39;ll use that clone as the starting point for the landing page.

In your instance, type **Service Porta** l in the Navigation menu. Click **Pages**.


4. Search for **\*index** (the \* in front a word stands for contains).


5. Open the **index** page.


6. On the top-right corner, click **Clone Page**.


7. Change the **Title** and **ID** to:


8. Click **Update**.
9. Now, create your own Service Portal!
In your instance, type **Service Portal** in the Navigation menu. Click **Portals**.


10. Click **New** to create a new portal.




11. Here you can see the main configuration possibilities of the Portal. Next to **Title** and **URL Suffix** you can set the pages of the portal. In this lab, you use the default page and configure it as you want. ill in the form with the following fields to create a new Service Portal:

Title: **Lightspeed IT Service Portal**         404 page: **404**
URL suffix: **itsp**         Catalog: **Service Catalog**
Homepage: **index\_lightspeed**         Main menu: **SP Header Menu**
Knowledge Base: **IT**         Theme: **Stock**
KB home page: **kb\_view2**
login: **landing**
12. Click **Submit** to create the portal.
13. Now test the portal! Open a new browser tab and navigate to
https://&lt;your instance&gt;.service-now.com/itsp
(you can use your admin credentials)

Notice that the created portal looks similar to the one in the first lab because you used the available standard pages/menu. Now, brand the portal to match the Lightspeed Enterprise Theme.

# Brand the Portal

1. Use the Service Portal Configuration to configure the portal. Service Portal Configuration is a powerful framework for designing and configuring a Portal.

In the Application Navigation bar, click **Service Portal Configuration**. This opens on a separate tab.

1. Click the menu option **Branding Editor** to open the Portal Designer.


2. The Branding Editor is used to brand the portal to your company colors; you also set the logo here.
3. Before starting, be sure the Lightspeed IT Service Portal is selected.


4. Download logo.png from [https://goo.gl/gKxJcg](https://goo.gl/gKxJcg)
5. Click **Upload an image** to set the company logo.


6. Go to the tab **Theme Colors**. We chose the following colors for the Navbar; feel free to be creative! You can also change the colors of the **Brand** and **Text** section.


7. Return to the tab **Quick Setup**. In the field **Tag Line color** , choose a color you like. In this example, the color white is selected. Notice that you could upload a background image here as well, but do not change the background image here. In the next lab, you&#39;ll learn a different method.


8. There is no need to save your changes as this is done automatically. You can close the browser tab.
9. Return to the portal (https://&lt;your instance&gt;.service-now.com/itsp) to see the changes.

## Lab 3.0 Design your Pages

## Lab Goal

The Portal is created! This lab explores the user experience, starting with the homepage. This must be created to direct users to an initial landing page when they access your portal. This lab explains how to:

- Adjust the homepage layout using the Designer
- Change/Configure the widget properties
- Publish data from any table within ServiceNow

# Adjust the Homepage

1. Return to the **Service Portal Configuration**.

1. Click the menu option **Designer** to open the Portal Designer.


2. The **Service Portal Designer** opens on a new tab. The initial view shows all pages available to the portal. Be sure the correct Portal is selected. You can change the active portal being worked on by clicking the  icon to change the active portal to your **Lightspeed IT Service Portal (itsp)**.



1. The active portal is now set to **itsp**.


2. Use the search box to find the **Index Lightspeed** page, select the **index\_lightspeed** page.


3. Before changing the portal&#39;s design, it&#39;s important to understand its structure (Containers, Rows, and Columns). A page consists of multiple Containers, and each container can contain one or more row(s); each row can contain a minimum of 1 column and a maximum of 6 columns. Below is a graphical example.

4. Now change the background image of the top container (Container 1).
Click on the outer dotted line to select **Container 1**.


5. Validate that the container is selected and not the row. If the row is selected, click **Container**.


6. Click the **pencil icon** to edit.


7. Download **background.png** from [https://goo.gl/gKxJcg](https://goo.gl/gKxJcg). Click the blue button **Upload an image**.

1. Select **background.png**
2. Click **Save**.

1. Also match the style of the 4 widgets below (Order Something, Knowledge Base, Get Help, and Community) to the uploaded background picture. First, select the container (Container 3) which carries the 4 widgets. Click **Edit** and change its background color to dark blue (#253047).


2. Click **Save**.

# Change/Configure the Widget Properties

1. Now adapt the style of the 4 widgets in the container. For each widget, do the following:

Hover the widget and click the **Pencil** button.
Change the **Glyph** icon to something you like.
Set the **template** to **Top Icon**.
Click **Save**.

2. Change the layout of the 4 widgets by dragging and dropping them in a different order.
3. The result should be like the example.

#
Publish Data from Any Table within ServiceNow

At the bottom of our page are some out-of-the-box widgets. It would be nice to create a widget to publish some relevant data for our end-users. In this example, you create a widget to show the **Open**** Requests** of that user and their approval stage.

1. Use the **Simple List** widget to publish data from the Request table within ServiceNow. In the **Widgets** tab, search for **simple** ; drag and drop the **Simple List** widget somewhere underneath the row of 4 widgets just changed.

1.
11.Hover over the widget, and click the **Pencil** button to edit it.


2. Complete the form as follows.

1. Click **Save**.
2. Open a new tab in the browser and navigate to the Service Portal:
https://&lt;your instance&gt;.service-now.com/itsp

The result of the widget should look like the example below.

# Filter Data

Note that you did not set the **Filter** field in the form as a result **all** open requests are displayed. You want to display only those requests for the specific user logged in.

1. Hover over the widget and click the **Pencil** button.

1. From the context menu (), click **Open in Platform**.


2. In the **Table &amp; Filter** tab:
Add an **and** condition where you set the **Opened By** &gt; **is (dynamic)** &gt; **me**
Click **Update**.

1. You can test the dynamic filter by viewing which **Request Items** are displayed when logging in with a different user (Abel or Aileen).

## Lab 4.0 Configure Widgets

## Lab Goal

After the homepage is created and the layout defined, you can now experiment with the widgets. This lab explains how to:

- Make a widget responsive (desktop/mobile)
- Control widget visibility by roles
- Create a widget

# Make a Widget Responsive

When developing a Service Portal, use the portal on all possible devices. However, on a Desktop you can show much more content on a single page than on a mobile device. The ServiceNow Portal allows you to make your widgets responsive to the environment they run on.

In this exercise, you add a video banner to the portal that displays when viewed on a **large screen** , but disappears if the page is viewed on a **mobile device**.

1. Make sure you are logged in as **admin**.
Go to the **Service Portal Configuration**.

1. Click the menu option **Designer** to open the Portal Designer.


2. Search for the **Index Lightspeed** page, to add a new container on the top of the page.
3. Before you can add the **Video Banner Widget** ,you need to add the container.Select the **container** object from the Layouts menu in the left menu bar, drag it onto the canvas and drop it at the top of the page above the top container.


4. Select the **column** object that is 12 columns wide, and drag and drop it into the container you just added.


5. Now add the **widget** to the page. Type the word **banner** in the search box **.** Drag and drop the **Banner Widget** in the container.


6. Select the newly added widget and click the **edit** symbol.


7. In the field **Banner Name** select the option **Video** and click **Save**.

1. Go to **Preview** and view the **Index Lightspeed** page in both **mobile** and **desktop** view.


2. Notice that you have now added the video banner to the top of the page. However, you have not yet configured it to disappear in **mobile view**. Another point of attention is that the video banner does not span the entire width of the screen.

Follow the steps below to correct both issues.

1. In **Service Portal Configuration** , click the menu option **Page Editor**.

1. Page Editor provides an easy-to-read tree-view of every element as it resides on the page.

The configuration of a page element (Container, Row, Column, Widget) are published directly under the tree-view when you click on it. Use this graphical view to visualize and edit the page elements.
2. Select the **Index Lightspeed** page.


3. Select Service Portal – Container 1.

1. Scroll to the configuration screen of this **container** and:

a.        Notice that the value of the field **Width** is set to **Fixed.** Change this value to **Fluid** in order         to make it scale properly with the width of the screen.

b.        To make the banner disappear when in mobile view, use the predefined
**        hidden-xs** CSS class. Set the value of the field **Parent class** to **hidden-xs**. As the name         suggests, this class causes the banner to be hidden when in mobile view. Other interesting         CSS classes you can experiment with are:



1. Click **Save**.

1. Return to the design view and **Preview** the **Index Lightspeed** page again in both **mobile** and **desktop** view (a refresh might be needed to enforce the changes).

Notice that in **mobile** view, the banner has disappeared and in **desktop** view, the banner nicely **scales** to the entire width of the page.

# Control Widget Visibility by Roles

# An important aspect in achieving an excellent user experience is personalizing the portal. Instead of creating a different portal for each user, you can control widget visibility by roles or role attributes. In this way, only the relevant widgets appear to the logged-in user. By showing only the relevant widgets to the user, you can create that personalized experience instead of a general experience (static HTML page).

In this example, you present the approval widget only to the users who have the role Manager because they are the only ones who need to approve the requests made by their team members.

1. Go to the Service Portal Configuration and select the **Page Editor**.

1. Select the **Index Lightspeed** page.


2. Select the widget **Approvals** in the graphical page-tree.


3. When you scroll down, you can see the properties of that widget. In the field **Roles,** configure which roles have visibility to the widget. Configure it such that only the Personas with the role **Manager** have access to this widget.


4. Scroll down and click **Save**.
5. Validate the visibility on the approval widget by logging into the Lightspeed Enterprise Service Portal as **Aileen** (Manager) and as **Abel** (Employee).

# Create a Widget

Now improve the user experience of the **Current Status** widget. The widget shows the availability status of the Business Services, the IT organization offers to Lightspeed Enterprise.

Make this widget interactive by adding the **Affected Too** button. When there is an outage on a Business Service, this lets users report that they are affected by the outage too. Clicking that button creates an **Incident** related to that outage.

1. The high-level steps to take are as follows:
  Copy existing widget
  Replace the widget on the page
  Extend the widget
    -  Place the new button
    -  Connect the button to a controller function with ng-click
    -  Write a controller function to invoke server side code (Create an Incident)
    -  Handle the case where an incident has been created (or was previously created)
2. Make sure you are logged in as **admin**.
Return to the **Service Portal Configuration**.

1. Click the menu option **Widget Editor**.

Widget Editor is a development framework that allows you to view and edit the source code for existing widgets, create new widgets, and update a widget&#39;s option schema.
2. **Copy existing widget** : In the **Widget Editor** , search forthe **Current Status** widget and open it.


3. A new window opens that displays all the different pieces that make up a widget in a single view (make sure the 4 check boxes are selected to show the relevant code). It is important to understand each of the lanes:

**HTML Template** – The HTML used to define the layout of the widget
**CSS** – The style sheet to manage the look and feel of the HTML template
**Client Script** – scripting that happens on the client. For example, when an element is clicked or the window loads
**Server Script** – Scripts that execute to interact with the Server, such as pull a property or database query


4. Notice the following message:


5.
39.First **Clone** the widget before editing it.

**Widget Name:** Affected Too
**Widget ID:** affected\_too


6. **Replace the widget on the page** : Click the menu option **Designer**.


7. Select the **Index Lightspeed** page.
Delete the **Current Status** widget from the page.


8. Drag and drop the **Affected Too** widget on the page.


9. **Extend the widget** : Return to the **Widget Editor** and select the **Affected Too** widget.

1. Make the changes to the code to reflect the desired functionality.
In the review session after this lab, we&#39;ll show you in detail the structure of the code, but for now, copy/paste all 3 sections (HTML Template, Client Script &amp; Server Script) from GitHub: [https://goo.gl/X6nOc9](https://goo.gl/X6nOc9).
2. **Save** the widget.

1. Test your newly created widget!
Open a new tab in the browser and navigate to the Service Portal:
https://&lt;your instance&gt;.service-now.com/itsp
2. Click the **I&#39;m affected too** button.

##
Bonus LAB Creating your own widget

## Introduction

In this bonus lab you will create your own custom twitter widget

_30 Minutes_

## Bonus Lab: Using low-code to create specific Widgets:

For this exercise, we&#39;re going to pull HTML code generated from Twitter, to add a twitter feed to your ServicePortal page.

First, we will navigate to twitter, and pull up your customer&#39;s twitter page, for this example, we&#39;re going to use the Life at ServiceNow twitter account: @LifeAtNOW

1. Open a web browser, and navigate to: [www.twitter.com](http://www.twitter.com)
2. Search for @lifeatNOW in the upper right corner

1. Towards the right side, you&#39;ll see three vertical dots, click on that, and select &quot;Embed this Profile&quot;:



1. Twitter offers two different options, select &quot;Embedded Timeline&quot;:



1. From here, we have the option of cutting and pasting the code, but as you can see on the lower half of the page, there is a preview example of what the code will display on the page. As is, the code will create a widget that is probably too large for your service portal page.
2. We will click on the &quot;set customization options&quot; link to open up additional options:

1. From here, we will set the Height to 500, and the Width to 400. This will be something that might require fine tuning in order to properly fit on your page. Luckily, this page still has a preview image at the bottom so you can see how your changes in height and width affects the size of the widget.

1. Click on &quot;update&quot; and on the next screen, click on the code text. This will automatically copy the code snippet. Here is the code for your convenience:
  1.
    1. &lt;a class=&quot;twitter-timeline&quot; data-width=&quot;400&quot; data-height=&quot;500&quot; data-theme=&quot;light&quot; href=&quot;https://twitter.com/LifeAtNOW&quot;&gt;Tweets by LifeAtNOW&lt;/a&gt; &lt;script async src=&quot;//platform.twitter.com/widgets.js&quot; charset=&quot;utf-8&quot;&gt;&lt;/script&gt;
2. Now, go to your instance, and go to the Service Portal Configurator, and select &quot;Widget Editor&quot;
3. From the Widget Editor, select &quot;Create a new Widget&quot;

1. You will be asked to name the widget. For this Lab, we&#39;ll call it &quot;Twitter Feed&quot; and click &quot;Submit&quot;:
2. In the next screen, we can copy and paste the code from Twitter underneath the &quot;&lt;!-- your widget template --&gt;&quot; line.

1. The &quot;&lt;!-- your widget template --&gt;&quot; line is not needed, and can be deleted.
2. Click on &quot;Save&quot; in the upper right hand corner

1. You have now successfully created a Widget using Low-Code!
2. You can now go to the &quot;Service Portal Configurator&quot;, select &quot;Designer&quot;, then select your page. For this example, we can go to our main Service Portal Index Page.
3. Find the &quot;Twitter Feed&quot; widget you just created along the left side by scrolling down, or typing &quot;Twitter Feed&quot; in the Filter Widget search field, and drag the widget into one of the available column.
4. Congrats! You now have your twitter feed on your service portal page!



# Why Service Portal?

1. Easy to create new portals for multiple lines of business.
2. Adding pages to portals is simple with the Portal Designer.
3. Page Editor provides a visual view of the layout of the portal for easy administration and control. No more guesswork over how the site is interconnected.
4. Responsive design ensures the portal is usable on all modern mobile devices with no additional configuration.
5. Interacts with the powerful underlying ServiceNow Platform. All platform components can be accessed from the portal. The possibilities are endless!
6. Modern web design frameworks are the foundation of the Portal (Bootstrap, AngularJS, CSS).
7. Advanced web designers can create rich web applications right on the ServiceNow Platform.