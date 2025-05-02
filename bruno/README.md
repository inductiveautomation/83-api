# Ignition HTTP API testing with Bruno

## How to use this repo

1. Download and install [Bruno](https://www.usebruno.com/).
2. `git clone` (or download + unzip) this repo.
3. In Bruno, click Collection > Open Collection, and select the `bruno/Ignition HTTP API` folder.
4. After selecting an endpoint, select "dev" from the environment dropdown in the top right.
5. *[Optional]* Choose "configure" from the environment dropdown and modify the gateway address or API token if needed.

## How to manually update this repo

If this repo is not up-to-date with the latest 8.3 routes, here's the process:

1. To ensure we get a clean import, move/rename your existing `bruno/Ignition HTTP API` to something like `bruno/OLD`.
2. Download the latest OpenAPI spec from your gateway.
   1. Login to your 8.3 gateway at `{YOUR_GATEWAY}/data/app/login`
   2. Navigate to `{YOUR_GATEWAY}/openapi`
   3. Click the Download button at the top of the page.
3. Import the OpenAPI spec into Bruno.
   1. In Bruno's Collections pane, click the "..." button, then click "Import Collection"
   2. Choose "OpenAPI V3 Spec" as the import type and select this repo's `bruno` folder as the import location. Files will be created at `bruno/Ignition HTTP API`.
5. Restore the environment(s) and collection variables from your backup created in Step 1.
   1. Copy the `collection.bru` file and the `environments` folder from the folder you moved/renamed in Step 1 into the new `bruno/Ignition HTTP API` folder created during import.
   2. *[Optional]* If there are other files in your backup that you want to bring in (modified endpoints, tests, etc.), do NOT copy them over until after the import.
