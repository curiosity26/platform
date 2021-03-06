# OroApiBundle

This bundle facilitates creation of different kinds of data APIs. It provides the default implementation that can be reused and easily tailored for any entity.

To achieve this, this bundle is implemented based on the following components: 

* [ChainProcessor](../../Component/ChainProcessor/) - Organizes data processing flow. 
* [EntitySerializer](../../Component/EntitySerializer/) - Provides the fast access to entities data.
* [Symfony Form](https://symfony.com/doc/current/components/form.html) - Provides a flexible way to map request data to entity object. 

Also, [FOSRestBundle](https://github.com/FriendsOfSymfony/FOSRestBundle) and [NelmioApiDocBundle](https://github.com/nelmio/NelmioApiDocBundle) are used for REST API.

**Notes**:

 - The main format for REST API is described at [JSON API](http://jsonapi.org/). Please be sure that you are familiar with it before you start creating REST API for your entities.
 - The auto-generated documentation and sandbox for REST API is available at `/api/doc/rest_json_api`, e.g. `http://demo.orocrm.com/api/doc/rest_json_api`. If you plan to use the sandbox, first make sure that you have generated an API key on the user profile page.
 - By default, only custom entities, dictionaries, and enumerations are accessible through the data API. For how to make other entities available via the data API, see [Configuration Reference](./Resources/doc/configuration.md).

Please see [documentation](./Resources/doc/index.md) for more details.
