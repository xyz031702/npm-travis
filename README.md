# Scantist npm/Travis CI Example

Shows a working setup for using Scantist to analyze the risk of project dependencies

## Travis CI Setup
The `.travis.yml` file has been modified to upload generated dependency data to Scantist:

```yaml
after_success:
  - bash <(curl -s https://scripts.scantist.com/staging/ci-travis-jar.sh)
```
