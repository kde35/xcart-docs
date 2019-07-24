---
lang: en
layout: article_with_sidebar
updated_at: '2017-01-29 01:26 +0400'
identifier: ref_kEKoAxJB
title: Product Class Attributes
categories:
  - User manual
published: true
order: 200
redirect_from:
  - /product_classes_and_attributes/managing_product_class_attributes.html
  - >-
    /product_classes_and_attributes/attributes/managing_product_class_attributes.html
  - >-
    /product_classes_and_attributes/attributes/attribute_scope/class_attributes.html
---
Product class attributes can be used to set up properties common for a group/class of products.  A store admin can add product classes and product class attributes either manually on a per-product basis or import them in bulk via a .csv file. 

Prior to assigning product class attribute(s) to a product a store admin must create and configure the related product class first. Product classes with no attributes configured for them are of no use.

X-Cart has 2 possible ways of creating and managing product classes and product class attributes that differ in means and actions that can be applied:
- via the **Classes & Attributes** section of the admin area, that allows to create, edit and delete product classes and add attributes to them. The changes done in this section will be applied store-wide.
  ![classes-attr.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/classes-attr.png)

- via the **Attributes** -> **Global** tab of any product details page, that allows to create product classes and assign them to products, as well as to add attributes to existing and newly created product classes and apply these attributes either store-wide or on a per-product basis, also it's possible to edit product-class attribute names store-wide and delete product-class attributes on a per-product basis here.
  ![classes-attr-product.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/classes-attr-product.png)

Read on the guides from this section to learn how to create and manage product class attributes in X-Cart.
{% toc %}

## Product Classes and Class-Attributes Management via the **Classes & Attributes** section

When you open the **Classes & Attributes** section (**Catalog** -> **Classes & Attributes**) in the store Admin area for the first time after the software installation, you are most likely to see a screen of the kind:

![attributes-listing.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/attributes-listing.png)

Here you see 1 sample {% link "global attribute" ref_HzMkgc0q %} and 3 sample product classes with attributes configured for them. 

The **Classes & Attributes** section (**Catalog** -> **Classes & Attributes**) section of the admin area gives a store admin the tools to create a product class, add attribute(s) or attribute groups to it, configure product class attributes, edit product class and product class attribute names and delete both product classes and product class attributes. 

Product classes creation and management via the **Classes & Attributes** section (**Catalog** -> **Classes & Attributes**) of the store Admin area is described in the {% link "Product Classes" ref_7bb4uhwg %} section of our Knowledge Base. Here we'll consider the product class attributes creation and management only.

### Adding Product Class Attributes to Product Classes

{% note warning %}
Adding product class attributes via the **Classes & Attributes** section of the Admin area (**Catalog > Classes & attributes**) implies that a related product class has been created beforehand as described in the {% link "Creating Product Classes" ref_6ieZHjOV %} guide of our Knowledge Base.
{% endnote %}

To add attribute(s) to an existing product class via the **Classes & Attributes** section follow the steps below:

1.  In your store's Admin area, go to the **Classes & attributes**section (**Catalog > Classes & attributes**).
2.  In the list of product classes, locate the product class you need to add an attribute to and click on the _Edit attributes (N)_ link opposite it:
    ![pc-attr-add-attribute-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-1.png)
    This opens a page where you will be able to manage attributes for this product class:
    ![pc-attr-add-attribute-1-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-1-1.png)
3.  On this page, click **New attribute**:
    ![pc-attr-add-attribute-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-2.png)
    A popup titled **New attribute** appears:
    ![pc-attr-add-attribute-3.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-3.png)
4.  Use the fields of the **New attribute** popup to provide information about the new attribute. Specify the following information:

    *   **Attribute**: Attribute name.
    *   **Attribute group**: Select a group name from the drop-down if this is applicable.
        {% note info%}
        Use the [Adding Groups to Product Class Attributes](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes.html#adding-groups-to-product-class-attributes "Product Class Attributes") part of this guide to learn how to join attributes into groups.
        {% endnote%}
    *   **Type**: Attribute value type (_Plain field_, _Textarea_, _Yes/No_).
        {% note info %}
        To choose a proper attribute value type for your attribute refer to the guides from {% link "Attribute Value Field Types" ref_5qw116xV %}.
        {% endnote %}
5.  Click **Next**. The attribute should be saved. 
    
    Now the popup is expanded so you can add/edit the values for this attribute:
    ![pc-attr-add-attribute-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-4.png)
6.  Click **New value** to configure the attribute values depending on the chosen {% link "attribute value field type" ref_5qw116xV %}. Add as many attribute values as you need.
    
    The screen below demonstrates adding a plain field value: 
    ![pc-attr-add-attribute-5.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-5.png)
7.  If you want some or all of the attribute value(s) you added for this product class to be applied automatically to all the products this product class will be assigned to in future, click the check-mark icon opposite the names of the related attribute values (the check-mark icon should turn green): 
    ![pc-attr-add-attribute-6.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-6.png)
8.  Once you're done with editing the attribute values, save the changes using the **Save changes** button:
   
    The attribute(s) will be added to the list of attributes of the related product class.
    ![pc-attr-add-attribute-7.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-7.png)


You can add as many attributes to one product class as you need. Once all required attributes have been created you can start [assigning this product class to products](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes.html#assigning-product-class-level-attributes-to-products "Product Class Attributes") in your store.

### Adding Groups to Product Class Attributes

In case a product class should have a considerable amount of attributes it makes sense to devide the attributes into groups to make the attributes representation to a customer structured and easy to persive.

![pc-attr-groups-cus.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-cus.png)

To add a group of attributes to a product class:

1. Locate the product class in quiestion in the Classes & attributes section (**Catalog > Classes & attributes**) in your store dmin area and click on __Edit attributes (N)__ link opposite it:
   ![pc-attr-add-attribute-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-1.png)
   This opens a page with the list of attributes for the selected product class:
   ![pc-attr-add-attribute-1-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-attribute-1-1.png)
2. On this page, click **Manage Groups**:
   ![pc-attr-groups-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-1.png)
   A popup titled **Manage attribute groups** appears.
   
3. Use the **New group** button to add as many attribute groups as you need:
   ![pc-attr-groups-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-2.png)
   
4. Click **Save changes** when you are done:
   ![pc-attr-groups-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-4.png)
   
5. The newly created groups will be added to the product class details page:
   ![pc-attr-groups-5.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-groups-5.png)

Now you can use these goups when [creating attributes](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes.html#adding-product-class-attributes-to-product-classes "Product Class Attributes") for this product class.

### Managing Product Class Attributes 

A store admin can check the list of attributes added to a product class and manage these attributes on a respective product class details page in the **Classes & attributes** section of the Admin area (**Catalog > Classes & attributes**).

To view the list of attributes a product class has a store admin should locate the respective product class in the **Classes & attributes** section of the Admin area  and click on _Edit attributes (N)_ link opposite it (where N stands for the numner of attribues a product class has).

<div class="ui stackable two column grid">
  <div class="column" markdown="span">![pc-attr-management-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-1.png)</div>
  <div class="column" markdown="span">![pc-attr-management-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-2.png)</div>
</div>

On a product class details page a store admin will sea a list of all attributes assigned to this product class with the respective attribute types by value.

Using the respective links(buttons) on the product class details page a store admin can:

1. [Add new attribute(s) to a product class](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes.html#adding-product-class-attributes-to-product-classes "Product Class Attributes")
2. [Create group(s) of attributes](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes.html#adding-groups-to-product-class-attributes "Product Class Attributes")
3. Edit attribute values and configuration
   
   To edit a product class attribute:
   *  In the list of product class attributes, locate the attribute you need to edit. 
   *  If you just need to change the attribute name, click inside the **Attribute name** field and edit the attribute name as you require. 
      ![pc-attr-management.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management.png)
   *  If you need to change the attribute values (or both the attribute name and values), click the **Edit** button:
      ![pc-attr-management-3.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-3.png)
      
      This will open a popup titled **Edit attribute values** where you will be able make the necessary changes.
      ![pc-attr-management-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-4.png)
      *  If you want some or all of the attribute value(s) to be applied automatically to all the products that will have this product class assigned in future, be sure to "enable" the check-mark icon opposite the names of the related attribute values (the check-mark icons should turn green):
         ![pc-attr-management-6.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-6.png)
      *  If you want to change the attribute values sorting use the **Cross** icons to re-arrange the values by grag-n-groping them:
         ![pc-attr-management-5.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-5.png)
      * If you want to apply the new sorting to all products that has this product class assigned by far, enable the **Apply sorting globally** checkbox:
        ![pc-attr-management-7.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-management-7.png)
        The **Apply sorting globally** setting affect the "active" attribute values only, i.e. the values that are marked with a green check-box and are automatically assigned to all products within this product class.

   *  Once you're done editing, click **Save changes**.

4. Make attribute(s) visible for product filter (works with {% link "Product Filter" ref_6e82A7rL %} addon only)
   
   Use the **Funnel with eye** icon opposite the product class attribute name to make this attribute visible in the product filters in the storefront.
   
5. Change attribute(s) order of apprearance
   
   Change the attributes order of appearance by drag-n-dropping the attributes with the help of a **Cross** icon.
   
6. Delete attribute(s)

   Use the **Trash** icon opposite a product class attribute name to marked the respective attribute for deletion.

Don't forget to **Save changes** when you are done with the attributes management.

## Product Classes and Class-Attributes Management via the **Attributes** -> **Global** tab of product details page

If speaking about product classes and product class attributes, the main purpose of the **Attributes** -> **Global** tab of a {% link "product details" ref_2D8wAeXP %} page is to give a store admin the tool to assign a product class to this particular product and to add it this way to a group of products that distinguish by properties.

It's generally accepted that the respective product classes and their attributes are created beforehand via the **Classes & attributes** section (**Catalog > Classes & attributes**) as described [above](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes.html#product-classes-and-class-attributes-management-via-the-classes--attributes-section "Product Class Attributes") because this is the most common way of product classes and product class attributes management.

However, if there is a need it's also possible to create a product class, assign it to a product and then add the necessary product class attributes to it directly in the **Attributes** -> **Global** tab of a product details page.

So all-in-all the **Attributes** -> **Global** tab of a product details page gives a store admin the tools for creating, assigning and managing product class attributes directly on a product page. The changes applied to product class attributes via the product details page can be applied both store-wide and at the product level only.

### Assigning Product Class Attributes to Products

{% note info %}
A product class assigned to a product must have product class attributes configured for it. Otherwise it's useless.
{% endnote %}

To assign a product class to a product:

1.  In your store's Admin area, locate the product you need to assign a product class to, open the product details and click on the **Attributes** tab:
    ![pc-attr-assign-1-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-assign-1-1.png)
    This will open a page where you can manage product class attributes for this product. 

2.  Chose __Global__ in the drop-down to access the subsection where you can add and assign {% link "global" ref_HzMkgc0q %} and product class attributes to this product.
    ![pc-attr-assign-2-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-assign-2-1.png)
3.  On the page that opens, click **Change** to assign a product class to this product:
    ![pc-attr-assign-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-assign-1.png)
4.  Chose the required product class from the drop-down:
    ![pc-attr-assign-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-assign-2.png)
5.  Click **Save changes** to assihn the chosen product class to the product
    ![pc-attr-assign-3.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-assign-3.png)
6.  The product class has been assigned to the product along with all product class attributes that are configured for it.
    ![pc-attr-assign-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-assign-4.png)
    The product class attributes that are available for this product class are listed below the product class name. 
    
If required a store admin can add new, edit and delete existing product class attributes directly on the product details page after a product class has been assigned to the product.

If any product attribute of the assigned product class comes with an undefined attribute value option, a store admin must assign an option to the respective attribute value for it to become available in product details in the storefront.

### Creating a New Product Class 

It may turn so that there is no required product class at the stage where it's necessary to chose the preferred product class from a drop-down on the **Attributes** -> **Global** tab of a product details page. In such a case a store admin has a possibility to create a new product class using the very same drop-down and assign this new product class to the product.

For this purpose:
1.  On the **Attributes** -> **Global** tab of a product details page, locate the Product class section and click the **Change** button:
    ![pc-attr-create-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-create-1.png)
    The product in question can either has no product class assigned to it or has some other product class assigned that should be changed for a new one.
2.  Choose the **New product class** option in the drop-down:
    ![pc-attr-create-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-create-2.png)
3.  Type in the name on a new product class in the field next to the **New product class** option:
    ![pc-attr-create-3.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-create-3.png)
4.  Click **Save changes** to assign the newly created product class to the product:
    ![pc-attr-create-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-create-4.png)

That's it! You've created a new product class and assigned it to a product in one and the same time:

![pc-attr-create-5.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-create-5.png)

Be warned that the newly created product class does NOT have any product class attributes configured for it. So you must proceed with adding attributes to this product class to make it working. Product class attributes can be added on the very same page the product class was created at. 

### Managing Product Class Attributes	

The **Attributes** -> **Global** tab of a product details page gives a store admin the tools to view the product class assigned to a product with a list of product class attributes configured for it, add attributes to both existing and newly created product classes, edit product class attributes and delete them.

![pc-attr-product-management.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-product-management.png)

Any changes to the product class attributes via the  **Attributes** -> **Global** tab of a product details page start with locating the required product in the **Products** seciton of the Admin area. Then it's necessary to open the **Attributes** -> **Global** tab of this product details page and check whether the product has the required product class assigned to it. If the product does not have a product class assigned, or needs to be assigned a different product class, take a moment to {% link "assign an appropriate product class to it" ref_EVqNSaZy#assigning-product-classes %}).

The page section intended for managing the product class attributes is titled based on the name of the product class according to the pattern "`<Product class name>` attributes" and gives a store admin the tools for: 

1.  **Adding New Attributes**

    To add a new product class attribute: 
    * click the **Add attribute** button opposite "`<Product class name>` attributes":
      ![pc-attr-add-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-1.png)
    * choose the attribute type in the drop-down:
      ![pc-attr-add-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-2.png)
    * Name the attribute and add attribute options. If necessary you can make {% link "multi-value attribute options " ref_465IZQg9 %} and add {% link "price and weight modifiers" ref_1t4DxHbf %} to them:
      ![pc-attr-add-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-add-4.png)
        
2. **Editing Product Class Attributes**

   1. To edit the attribute name, hover your cursor over the attribute you want to change (the **Attribute name** field will become visible), click inside the **Attribute name** field and edit the attribute name as you require:
      ![pc-attr-edit-1.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-edit-1.png)
   2. To edit the values of product class attribute options (the options that have been added automatically along with the product class assignment):
      * click on the attribute option name to change it;
        ![pc-attr-edit-2.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-edit-2.png)
      * click on the drop-down errow next to the attribute option name to choose another option from the list of suggested;
        ![pc-attr-edit-3.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-edit-3.png)
      * click on the _Modifiers_ link next to the attribute option name to add {% link "Price and Weight Modifiers" ref_1t4DxHbf %};
        ![pc-attr-edit-4.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-edit-4.png)
        
        {% note info %}
        In case _Modifiers_ are added to the existing product class attribute option(s) and are applied globally (with the **Apply attribute value changes for all the products** setting enabled) the changes will affect only the products with the corresponding attribute option(s) enabled. All products that has the corresponding attribute option(s) disabled will stay as is.
        {% endnote %}
        
      * click on the _Trash_ icon opposite the attribute option to delete it.
        ![pc-attr-edit-5.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-edit-5.png)
    3. To add a new attribute option, locate the unconfigured attribute option line for this attribute (usually the very last empty line in the attribute values list) and either enter the preferred option value directly in the attribute option field or choose a value from the list of suggested using the drop-down errow.
       ![pc-attr-edit-6.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-edit-6.png)
        
3. **Deleting Product Class Attributes for a Product**
   
   To delete a product class attribute find the attribute you want to delete and click on the **Trash** icon opposite its name. The attribute will be marked for deletion.
   
   ![pc-attr-delete.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/pc-attr-delete.png)

   {% note info %}
   Deleting a product class attribute on the product details page results in removing all existing attribute options and affects this very product only. The product class attribute itself becomes unconfigured for this particular product and thus not visible for it in the storefront.
   
   To remove the attribute as a whole for all the products within this product class, use the ["Classes  & Attrubutes" page](https://kb.x-cart.com/product_classes_and_attributes/attributes/attribute_scope/class_attributes.html#managing-product-class-attributes "Product Class Attributes").
   {% endnote %}
   
When you are done with the product class attributes management specify whether the changes should be applied to this particular product only or to the product class as a whole (affects all products with this product class assigned):

![apply-changes-globally.png]({{site.baseurl}}/attachments/ref_kEKoAxJB/apply-changes-globally.png)

*   If the **Apply attribute value changes for all the products** setting is turned OFF the changes you made will be applied to this particular product only.
 
*   If the **Apply attribute value changes for all the products** setting is turned ON the changes you made will affect all products with the same product class assigned, i.e. the changes will be applied on a product-class level.
    
   Note that when you apply attribute values globally, they are applied only to products that have the same product class assigned at the time you save the changes. Any products to which the product class in question will be assigned at a later time will _not_ get these values automatically.

Click **Save changes** to make the changes active.


_Related pages:_

*   {% link "Product Classes and Attributes" ref_T90ZcEpP %}
*   {% link "Product Classes" ref_7bb4uhwg %}
*   {% link "Types of Product Attributes - by Scope" ref_uaJk8ete %}
*   {% link "Multi-Value Attributes (Product Options)" ref_465IZQg9 %}
*   {% link "Price and Weight Modifiers" ref_1t4DxHbf %}