# google-cloud-vision

Google Cloud Vision allows easy integration of vision detection features
developer applications, including image labeling, face and landmark
detection, optical character recognition (OCR), and tagging of explicit
content.

- [google-cloud-vision API documentation](http://googlecloudplatform.github.io/gcloud-ruby/#/docs/google-cloud-vision/google/cloud/vision)
- [Google Cloud Vision documentation](https://cloud.google.com/vision/docs)

## Authentication

This library uses Service Account credentials to connect to Google Cloud services. When running on Compute Engine the credentials will be discovered automatically. When running on other environments the Service Account credentials can be specified by providing the path to the JSON file, or the JSON itself, in environment variables.

Instructions and configuration options are covered in the [Authentication Guide](https://googlecloudplatform.github.io/gcloud-ruby/#/docs/google-cloud-vision/guides/authentication).

## Example

```ruby
require "google/cloud"

gcloud = Google::Cloud.new
vision = gcloud.vision

image = vision.image "path/to/landmark.jpg"

landmark = image.landmark
landmark.description #=> "Mount Rushmore"
```

## Supported Ruby Versions

This library is supported on Ruby 2.0+.

## Versioning

This library follows [Semantic Versioning](http://semver.org/).

It is currently in major version zero (0.y.z), which means that anything may change at any time and the public API should not be considered stable.

## Contributing

Contributions to this library are always welcome and highly encouraged.

See the [Contributing Guide](https://googlecloudplatform.github.io/gcloud-ruby/#/docs/guides/contributing) for more information on how to get started.

Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms. See [Code of Conduct](../CODE_OF_CONDUCT.md) for more information.

## License

This library is licensed under Apache 2.0. Full license text is available in [LICENSE](../LICENSE).

## Support

Please [report bugs at the project on Github](https://github.com/GoogleCloudPlatform/gcloud-ruby/issues).
Don't hesitate to [ask questions](http://stackoverflow.com/questions/tagged/gcloud-ruby) about the client or APIs on [StackOverflow](http://stackoverflow.com).