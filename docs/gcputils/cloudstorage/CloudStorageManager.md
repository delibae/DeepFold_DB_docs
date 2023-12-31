# gcputils.cloudstorage.CloudStorageManager

The `CloudStorageManager` class provides an interface to interact with Google Cloud Storage service. It requires the Google Cloud Storage bucket name during initialization.

## Attributes

- `bucket_name (str)`: The Google Cloud Storage bucket name.

## Methods

### `__init__`

Initializes a new instance of the `CloudStorageManager` class.

**Parameters:**

- `bucket_name (str)`: The Google Cloud Storage bucket name.

### `list_blobs`

Lists all the blobs in the bucket.

**Returns:**

- `List[str]`: A list of blob names in the bucket.

### `download_blob`

Downloads a blob from the bucket.

**Parameters:**

- `blob_name (str)`: The name of the blob to download.
- `destination_dir (str)`: The directory where the downloaded blob will be stored.

### `download_bucket`

Downloads all blobs from the bucket.

**Parameters:**

- `max_workers (int)`: The maximum number of worker threads that will be used to download blobs.
- `destination_dir (str)`: The directory where the downloaded blobs will be stored.
