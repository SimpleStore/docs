# Assets

Simple store supports the upload, storage and management of assess \(files\) that can be associated with Products and Categories.  Examples of assets include: jpg, gif, png, pdf.

### Portal View

#### Accessing Assets 

Assess the Assets screen in the console via the console navigation bar.

![](../../.gitbook/assets/image%20%2824%29.png)

#### Add New Asset

Click Upload File to upload and create the new asset.

![](../../.gitbook/assets/image%20%2815%29.png)

Specify a Title, Description and Access Permission.

Access Permission allow an assets to be defined as Public or Private

Drag and Drop the asset to upload.

![](../../.gitbook/assets/image%20%2816%29.png)

Click **Submit**.

#### Edit Assets

Assets can be accessed by clicking on the main asset screen:

![](../../.gitbook/assets/image%20%2835%29.png)

File Details can be edited.

![](../../.gitbook/assets/image%20%2839%29.png)

Click **Save** to commit your modifications.

Assets can be deleted by clicking the **Delete** button.

### Asset Properties

#### Folders

Assets can be stored in a hierarchy of folders.

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| folderId | Unique Identifer for the Folder |
| version | An incremental version number tracking changes to the folder configuration |
| name | Name |
| parentId | A parent folder identifier to support the creation of a hierarchical/tree based structure of related folder |
| attributes | Attributes are a list of Key/Value to support customisation of a folder |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "folderId": "string",
  "version": "string",
  "name": "string",
  "parentId": "string",
  "attributes": {}
}
```
{% endtab %}
{% endtabs %}

#### Files

Files represent the range of assets that can be stored and managed.

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| fileId | Unique Identifer for the File |
| version | An incremental version number tracking changes to the folder configuration |
| title | Title of Image |
| description | Description |
| contentType | Content-Type of file |
| fileName | File Name |
| length | File Length |
| width | Width of File \(images\) |
| height | Height of File \(images\) |
| accessUrl | Access Url |
| accessPermission | Access Permission |
| attributes | Attributes are a list of Key/Value to support customisation of a folder |
| isActive | Is Active |
| folderId | Reference to Containing Folder Id |
| edgeUrl | Edge Url |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "fileId": "string",
  "version": "string",
  "title": "string",
  "description": "string",
  "contentType": "string",
  "fileName": "string",
  "length": 0,
  "width": 0,
  "height": 0,
  "accessUrl": "string",
  "accessPermission": 0,
  "attributes": {},
  "isActive": true,
  "folderId": "string",
  "edgeUrl": "string"
}
```
{% endtab %}
{% endtabs %}

