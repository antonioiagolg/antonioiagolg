* Migrations are a delicate topic. First thing to check is the data schema.

* Data optional -> now required: In this scenario we must provide a default value for thes fields. Clients should be aware beforehand that dat is required and they should provide the correct data in a specific period.

* Data required -> optional: In this scenario we have less noise, as in the previous schema we must have the data.

* No field -> new required: Same approach as item 2, observing the default data to no break the requirements.

* No field -> new optional: Same approach as item 2, observing the defautl data or nullable value.

* Data with one type -> same data in another type: For example, we have a data represented as string, but for any reason the data must be an object -> We may keep the old data on the new structure for backward compatibility
