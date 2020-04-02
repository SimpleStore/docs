# Categories

Specials define rule based price modifiers to support discounting of products.

Specials can be either a **percentage** or a **fixed** amount.

Specials apply for a specified date range

Specials can be applied to:

* **Products** - specific products
* **Categories** - all Products assigned to a category
* **Collections** - all Products assigned to a collection

#### Specials Properties

| Element | Description |
| :--- | :--- |
| Special Id | Internal Identifier for the special |
| Name | Name for the special |
| Description | Description for the special |
| Special Type | Percentage or Fixed Amount |
| Amount | Amount of special, unit based on Special Type |
| Start Date | Start date for the special |
| End Date | End date for the special |
| **Rules** |  |
| Categories | Categories that the special applies to \(see [Categories](categories.md)\), if a Product is assigned to these categories then the special is applied |
| Collections | Collections that the special applies to \(see [Categories](categories.md)\), if a Product is assigned to these categories then the special is applied |
| Products |  |
| Attributes | One or more key/value pairs to support customisation of specials |

