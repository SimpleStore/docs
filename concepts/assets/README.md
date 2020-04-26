# Assets

Simple store supports the upload, storage and management of assess \(files\) that can be associated with Products and Categories.  Examples of assets include: jpg, gif, png, pdf.

### Portal View



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

