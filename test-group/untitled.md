# Owners portal description \(too detailed\)

### Edit the Dummy Table

In order to make the Owner's portal more useful to admin users, you can set up data tables similar to the Users table that already set up on the owner page.

The easiest way to do this is to edit the Dummy table which is hidden below the User's table on the **Owner** page.

Here's how you can do it:

1. Open the **owner** page in the Bubble editor \(e.g. https://bubble.io/page?type=page&name=owner&id=YOUR-APP-ID&tab=tabs-1\).
2. Select the group called **Group Dummy Tab** on the **owner** page.
3. Change the visible fields for this group, including:
   1. Title \(is "Dummy" by default\)
   2. Set up the placeholder text or image for when no items are found. This is found in the group called "**group no entries**", and should be something like "This User table is empty"
   3. Change the datatype of the **RepeatingGroup Dummy** to the type of data that you'd like to display in this table.
   4. Set up the columns of the table: column names and the actual content. For the column content, you'll need to use some dynamic data, showing for example`Current Cell's Tweet's Text's number of characters`  in order to see the total number of characters for each tweet if you're creating a table of tweets.
4. Set up the workflows for this group, including:
   1. Action for Add Dummy button
   2. Action for Download Data button
5. Set up the Search for objects in the **RepeatingGroup Dummy**. You'll need to search for whatever type of data that you'd like to display, and if you want any sort of filtering on that search, you'll also need to add the **"Search by Name"** input as a data source on the search.
6. Change the Nav settings on **FloatingGroup B** to show this element. You'll need to unhide **Group Nav 7 tab** \(in the portal sidebar navigation\) and give the tab a different text to display \(e.g. "Tweets"\). For more context, see the screenshots below.

After each change you make here, make sure to view the web page in version-test in order to check whether it works as expected.

### Adding additional tabs to the Owner's Portal

In order to make the Owner's portal more useful to admin users, you can set up data tables similar to the Users table that comes with the template.

In order to do this, it'd be helpful to have experience working with the Bubble design tab. 

1. Open the **owner** page in the Bubble editor \(e.g. https://bubble.io/page?type=page&name=owner&id=YOUR-APP-ID&tab=tabs-1\).
2. Select the group **Group Users** on the **owner** page.
3. Open the **Edit** dropdown from the Bubble toolbar \(near the top left of the page on the top bar\).
4. Select **Copy with Workflows**.
5. Select **Group Placeholder** and decrease its height by 380, increase its Y position by 380 to make room for the new group.
6. Open the **Edit** dropdown again and select **Paste with Workflows.**
7. Move the newly pasted group to below the **Group Users** \(or whatever the last data table is\) ****, with the same X position. Make sure the group isn't overlapping with either the **Group PLACEHOLDER** or the group above it. 
8. Edit the fields of the table and set up a tab for this group as described in the above Dummy Table example. 
9. In order to get the tab working for this new table, you'll need to go through 2 additional steps.
   1. Select the new group you've just created and got to the conditional tab. Make the conditional logic refer to **Group Nav 8 tab** instead of **Group Users tab 6.** See screenshot below for more context.
   2. Select **Group** **Nav 8 tab**, make it visible, and give it a new text, just like you would do for the Dummy Table with Group Nav 7 tab. 

You're all set! If this text isn't clear, you can post in the Bubble forum to ask for help setting this up.



x

