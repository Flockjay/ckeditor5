# CKEditor 5 Fork

The original repository can be found at [ckeditor/ckeditor5](https://github.com/ckeditor/ckeditor5).

## Modified Packages

The following packages have been customized in this fork:

-   `packages/ckeditor5-build-classic`
-   `packages/ckeditor5-image`
-   `packages/ckeditor5-media-embed`

## Development

### Testing

To run tests for the modified packages:

```bash
yarn run manual --files=build-classic|image|media-embed
```

### Building

To build the modified packages:

```bash
cd packages/<package-name>
yarn run build
```

### Frontend Integration

After building and merging changes:

1. Update the commit hash in frontend application to use the latest version
2. Rebuild frontend application:
    ```bash
    yarn install --ignore-scripts
    yarn start:dev
    ```

## License

Licensed under the terms of [GNU General Public License Version 2 or later](http://www.gnu.org/licenses/gpl.html). For full details about the license, please check the `LICENSE.md` file or [https://ckeditor.com/legal/ckeditor-oss-license](https://ckeditor.com/legal/ckeditor-oss-license).
