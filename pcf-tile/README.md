# Generate a PCF Tile

1. Install the tile-generator python package. Note: tile-generator requires Python 2, and will not work with Python 3. We recommend using a virtualenv environment to avoid conflicts with other Python packages:

  ```
  virtualenv -p python3 tile-generator
  source tile-generator/bin/activate
  pip install tile-generator
  ```

  This will put the tile and pcf commands in your PATH.

1. Install the [BOSH CLI](https://bosh.io/docs/bosh-cli.html)

1. Under the folder `pcf-tile`, execute below command.

  ```
  ./generate-tile.sh
  ```

  Note:
    * Build a major version: ./generate-tile.sh -major
    * Build a minor version: ./generate-tile.sh -minor
    * Build a patch version: ./generate-tile.sh

1. You can find meta-azure-service-broker-`VERSION`.pivotal under the folder `product`.
