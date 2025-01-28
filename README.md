# Sharepoint for Zoho CRM: Extended for Custom Module

Here's a breakdown of the process of configuring the extension to a custom module:
1. In the custom module where you need the extension's functionalities, create three custom fields: SiteId, DriveId, and DriveItemId.
2. Download the ZIP (SP_custom_module) file from this repository.
3. Unzip the file and navigate to the following path within the unzipped folder: *SP_Custom_Feature* > *app* > *js* > *foldersync.js*.
4. Open the foldersync.js file in any JavaScript editor.
5. Under the variable *Constants*, you'll find the siteId, driveId, and driveItemId keys. Provide the API names of the custom fields you created as values.
6. In *folderPath*, provide the SharePoint folder URL related to this custom module. This folder is where the extension fetches or pushes files.
7. The dynamic folder directory has to be given in ${field_API_name} format.
8. Save the foldersync.js file.
9. Create a widget and replace the default .js file in the app folder with this foldersync.js file. 
10. Associate the extension with your Zoho CRM by following the documentation provided.
    - [Create a widget](https://help.zoho.com/portal/en/community/topic/extension-pointers-working-with-widgets-to-power-up-extension-capabilities-part-1)
    - [Associate the widget to Zoho CRM](https://www.zoho.com/crm/developer/docs/widgets/usage.html)

Once the widget is created, you'll be able to manage files in Zoho CRM and SharePoint using the extension's functionalities. If you need more guidance, our comprehensive [help documentation](https://help.zoho.com/portal/en/kb/crm/extensions/marketing/articles/sharepoint-for-zoho-crm) is always available.

If you have any further questions, please email us at [support@zohomarketplace.com](mailto:support@zohomarketplace.com), and we will be happy to assist you.
