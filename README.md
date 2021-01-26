
Optimistic locking seems not to work correctly when updating an domain class.

The version property  value in the domain class is overwritten by the database value before saving the entity.
Therefore the version property has always the newest (highest) value and the optimistic lock exception is never thrown. 
