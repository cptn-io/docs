---
sidebar_position: 2
---

# Contributing Apps

Any user can contribute Apps to the community. Approved apps will be automatically downloaded to all cptn.io instances and can be readily used in any Pipelines.

You can contribute any Destinations or Transformers defined on your instance as Apps. 

Our git repo for shared apps is available at https://github.com/cptn-io/apps

## To contribute Apps
1. Login to your instance.
2. Navigate to the Transformer or the Destination details page that you'd like to share with the community.
3. Ensure that the Script doesn't have any credentials, private or senstitive information. The configuration values in a Destination are automatically stripped.
4. Click **Export as App** button.
5. A new JSON file will be downloaded.
6. Review the contents of the JSON file. Update the name, logoUrl if required. We use brand logo icons at https://simpleicons.org/ for the apps, if applicable. SimpleIcons are hosted on CDN and accessible via https://cdn.simpleicons.org/ (e.g. https://cdn.simpleicons.org/twilio)
6. Visit https://github.com/cptn-io/apps. Create a new branch and push the JSON file to the branch. 
7. Create a new pull request for the newly created branch to merge to **dev** branch. Provide any additional details on the PR to help with review. If you need to share any sensitive information or credentials for testing the App, send an email to support@devraven.io with the details.
8. We will review the PR, test the app and will merge it into main. 

## Updating previously shared Apps

To update a previously published App:
1. Login to the instance.
2. Navigate to the Destination or the Tranformer to be updated.
3. Do the required changes to the Script or Configuration.
4. Click **Export as App** button.
5. A new JSON file will be downloaded.
6. Review the contents of the JSON file. Update the name, logoUrl if required.
7. Ensure that the value for the property **key** is same as the previously published app.
8. The value for the property **hash** must be different.
9. Follow the instructions as above to create a pull request for updating the app content.

## License

Any Apps shared will the community are treated as MIT licensed code.

:::danger
Do not share any properietary code or code available under different license with the community.
:::