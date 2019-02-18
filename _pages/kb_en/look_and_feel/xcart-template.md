---
lang: en
layout: article_with_sidebar
updated_at: '2019-01-28 10:39 +0400'
identifier: ref_2qN1oWni
title: Overview of a Template Structure
order: 100
published: true
---
X-Cart skin is a template that determines the way your online store looks and feels. Different skins have different styles and layouts, and offer a different experience for your customers. 

X-Cart offers 5 skins out-of-the-box and over 55 skins that can be downloaded and installed from the Marketplace. The store admin area uses the X-Cart Standard skin by default. As for the customer storefront you can change the skin used there depending on the impression you want your store to have on your customers.

Although each skin is different, all of them have some common features. All skins let you use the same types of pages, and all pages include some standard elements. 

A combination of page elements and page types make up a theme's structure.

## Page elements

All pages of a skin include these page elements:

{:.ui.compact.celled.small.padded.table} 
|Element|Description| 
|Header|The content area that appears at the top of each page of your store. The header usually includes your store's name, your logo, main menu navigation, customer account link and cart icon.|
|Body|The area on every page of your online store between the header and the footer. Unlike the header and footer, which are fixed elements that stay the same on every page, the body of the page is dynamic, and contains content that changes depending on the page that you are on.|
|Navigation| A menu or a block of menus that provide a way for customers to explore or move around your online store. The main menu navigation is included in the header of a skin.|
|Footer|The content area that appears at the bottom of every page of your store. The footer might include menus, social media icons, contact information, or a newsletter signup.| 

## Page types

X-Cart uses 2 main page types - static pages and dynamic pages.

Static pages contain the same prebuilt content each time the page is loaded, while the content of dynamic pages is generated on-the-fly depending on the actions performed by a customer on your site. 

All static pages are managed through the **Content** -> **Pages** section of the store admin area where it's possible to create a new static page, enable/disable it and manage the page content. 

Dynamic pages are more complex and can't be managed that simple as static pages because they are hardcoded in the store template. Hence the only changes a store admin can add to dynamic pages are the changes added via the {% link "Theme Tweaker" ref_2Kfe2OX6 %} facilities. Also it's possible to use the **Custom CSS & JS** section of the store admin area (**Look & Feel** -> **Custom CSS & JS**) to add a custom code to a template. All custom code changes of the dynamic pages are recorded in the **Edited templates** section of the store admin area (**Look & Feel** -> **Edited templates**). 

Dynamic page loading usually takes more time than a staic one. Hence caching is used to deliver faster page load times, reduce hosting costs, and improve overall user experience by improving the overall page speed.

All skins include these types of pages:

{:.ui.compact.celled.small.padded.table} 
|Page|Description|
|Home|	The home page is the main page of your online store. It's a dynamic page and this is the default page that opens when a customer visits your website.|
|Category| A dynamic page that shows all of the products that you have included in a given category.|
|Product|A dynamic page that shows a product and its variants. It includes product images, pricing information, a product description, and an Add to cart button.|
|Cart|A dynamic page that shows a summary of all of the products that a customer has added to the cart, a subtotal and a total price for the order, and a Checkout button that directs customers to secure checkout pages.|
|Search|A dynamic page that includes a search bar and a list of search results.|
|Contact Us| A static page that includes your store contact details and a form that customers can use to contact you.|
|Customer| A block of dynamic pages that include the customer registration page, the customer login page, and the customer account page. The customer account page includes the customer's profile, messages, wishilist, shipping address book and information about any existing orders.|
