# ocspbuilder

A Python library for creating and signing online certificate status protocol
(OCSP) requests and responses for X.509 certificates.

 - [Related Crypto Libraries](#related-crypto-libraries)
 - [Current Release](#current-release)
 - [Dependencies](#dependencies)
 - [Installation](#installation)
 - [License](#license)
 - [Documentation](#documentation)
 - [Continuous Integration](#continuous-integration)
 - [Testing](#testing)
 - [Development](#development)

## Related Crypto Libraries

*ocspbuilder* is part of the modularcrypto family of Python packages:

 - [asn1crypto](https://github.com/wbond/asn1crypto)
 - [oscrypto](https://github.com/wbond/oscrypto)
 - [csrbuilder](https://github.com/wbond/csrbuilder)
 - [certbuilder](https://github.com/wbond/certbuilder)
 - [crlbuilder](https://github.com/wbond/crlbuilder)
 - [ocspbuilder](https://github.com/wbond/ocspbuilder)
 - [certvalidator](https://github.com/wbond/certvalidator)

## Current Release

0.10.0 - [changelog](changelog.md)

## Dependencies

 - [*asn1crypto*](https://github.com/wbond/asn1crypto)
 - [*oscrypto*](https://github.com/wbond/oscrypto)
 - Python 2.6, 2.7, 3.2, 3.3, 3.4, 3.5, pypy or pypy3

## Installation

```bash
pip install ocspbuilder
```

## License

*ocspbuilder* is licensed under the terms of the MIT license. See the
[LICENSE](LICENSE) file for the exact license text.

## Documentation

[*ocspbuilder* documentation](docs/readme.md)

## Continuous Integration

 - [Windows](https://ci.appveyor.com/project/wbond/ocspbuilder/history) via AppVeyor
 - [OS X & Linux](https://travis-ci.org/wbond/ocspbuilder/builds) via Travis CI

## Testing

Tests are written using `unittest` and require no third-party packages:

```bash
python run.py tests
```

To run only some tests, pass a regular expression as a parameter to `tests`.

```bash
python run.py tests build
```

## Development

To install required development dependencies, execute:

```bash
pip install -r dev-requirements.txt
```

The following commands will run the linter and test coverage:

```bash
python run.py lint
python run.py coverage
```

The following will regenerate the API documentation:

```bash
python run.py api_docs
```

After creating a [semver](http://semver.org/) git tag, a `.tar.gz` and `.whl`
of the package can be created and uploaded to
[PyPi](https://pypi.python.org/pypi/ocspbuilder) by executing:

```bash
python run.py release
```
