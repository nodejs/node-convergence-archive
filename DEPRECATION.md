# Deprecation Policy

## Stage 1

1. The technical committee decides to deprecate an officially supported API.  
2. The function is changed to the `util.deprecate` function with a message that indicates the intent for removal and a 
suggested replacement API to use, if there is one.
3. The API documentation is updated to reflect that the API functionality will be removed in the future. 
4. The changed API is released with the minor version being incremented.
5. An issue is filed to delete the deprecated API


## Stage 2

1. During the next major release since the release of the deprecated API, the API should be deleted.  The 
related issue from step 5 stage 1 is closed.
2. The API documentation is updated to reflect that the API functionality has been deleted.
3. Release notes are created to guide developers on the breaking change and how to upgrade.
4. The major version is incremented and a release is issued
5. An issue is filed to remove the note from the API documentation


## Stage 3

1. Remove the note from the API documentation and close the issue from step 5 stage 2.
2. The documentation change can go out with any future release
