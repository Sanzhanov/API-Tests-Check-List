# API-Tests-Check-List*

## POST requests
* All fields filled with valid data
* Only required fields are filled
* Not all required fields are filled
* No field is filled
* Empty json
* Validation of data in the fields (correct and incorrect data)

## GET requests
* Request data by valid ID
* Request data for a non-existent ID, but in a valid format
* Request data for invalid ID
* Completed list
* Empty list (if possible)
* Pagination in the list (limit, offset)
* Get a list with a limit on the number of entries
* Get a list starting from the specified number
* In case of passing parameters with an incorrect value, 400 is returned with a description of the error in the response body
* If offset is negative, the list of users is returned starting from the first position
* If offset does not exist, an empty list of users is returned
* List sorting

## PUT requests
* Update with valid ID
* Update by non-existent ID
* Update by invalid ID
* Partial update (not all fields are present in JSON)
* Validation of fields (correct and incorrect data)

## DELETE requests
* Removing of existing object
* Removing of already deleted object
* Removing by non-existent but valid ID
* Removing by invalid ID
* Removing and re-adding the same entity (if there are unique fields)

1. Checking response statuses
2. Checking for all possible errors
3. Other specific checks in case of complex logic

**list in progress, thetefore if you've found a mistake pls send me a pull request*
