# Pimcore News
Pimcore News Plugin. It's also possible to generate [custom entry types](docs/20_EntryTypes.md) like Press, Blog...

## Requirements
* Pimcore 5. Only with Build 108 or greater.

#### Pimcore 4 
Get the Pimcore4 Version [here](https://github.com/dachcom-digital/pimcore-news/tree/pimcore4).

## Installation

**Composer Installation**  
1. Add code below to your `composer.json`    
2. Activate & install it through backend

```json
"require" : {
    "dachcom-digital/news" : "dev-master",
}
```

## Important to know
- The detail url is based on the title for each language. If the detail url field is empty, the title will be transformed to a valid url slug.
- The News Bundle will install two classes (`NewsEntry` and `NewsCategory`). If you're going to modify them, please be sure that you're follow our [upgrade notes](UPGRADE.md) in case we're changing the class structure.

## Good to know
- News can be placed at any place on your website through the news area element. Use it as list, latest or even as a custom layout.
- The detail page always stays the same (see static route), no matter where you placed the area element.
- It's possible to override the detail url in the news object.

## Extending News Object
- *Meta Information* Tab: Extend News with [classification store](https://www.pimcore.org/docs/latest/Objects/Object_Classes/Data_Types/Classification_Store.html) data.  
- *Relations & Settings* Tab: Extend News with [Object Bricks](https://www.pimcore.org/docs/latest/Objects/Object_Classes/Data_Types/Object_Bricks.html).  

### Further Information
- [Head Meta Generator](docs/10_HeadMetaGenerator.md)
- [Link Generator](docs/11_LinkGenerator.md)
- [Related Entries Generator](docs/12_RelatedEntriesGenerator.md)
- [The Amazing Entry Types](docs/20_EntryTypes.md)
        
## Widgets
TBD

## Copyright and license
Copyright: [DACHCOM.DIGITAL](http://dachcom-digital.ch)  
For licensing details please visit [LICENSE.md](LICENSE.md)  

## Upgrade Info
Before updating, please [check our upgrade notes!](UPGRADE.md)
