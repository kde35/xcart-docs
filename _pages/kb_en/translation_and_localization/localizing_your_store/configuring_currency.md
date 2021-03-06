---
lang: en
layout: article_with_sidebar
updated_at: '2019-02-27 12:06 +0400'
identifier: ref_2dx6iFtL
title: Configuring Currency
order: 110
published: true
---
To configure currency:

1.  Go to the Currency section of your store's Admin area (**Store setup** > **Localization**).
    ![currency.png]({{site.baseurl}}/attachments/ref_2dx6iFtL/currency.png)
2. Use the settings in this section to adjust the currency parameters for your country:
   * **Hide trailing zeros in fractional part** : If this option is enabled zeros in fractional part will be hidden for prices with decimals, e.g. a price of $1234.00 will be displayed as $1234, at the same time a price of $1234.56 will be displayed as is - $1234.56.
   * **Store currency** : Choose your store currency from the list.
   * **Format** : Set the appropriate format of the prices representation.
   * **Prefix** : The field is defined automatically based on the chosen **Store currency** field value.
   * **Suffix** : The field is defined automatically based on the chosen **Store currency** field value.
3. **Save changes** to submit the currency settings.

{% note info %}
If you want the prices to be displayed in a currency matching a customer's location use the {% link "Multicurrency Addon" ref_2tPJubPU %}
{% endnote %}
