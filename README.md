# Node Cookbook

## Pre-requisites

- Chef
- Git
- NodeJs
- Nginx
- pm2
- npm
- AWS CLI v2
- Virtual Box

## Chef

Chef is a configuration management tool. Using Chef, you can provision cookbooks by giving recipes packages you will need to use in your environment, while being to safely test that everything is installed. This will allow you to easily create an AMI which has a standardised and provisioned environment.

## Commands

Follow the commands below to run the cookbook.

### Cloning the repo

To clone this repo:
```
$ git clone git@github.com:hovell722/NodeCookbookStarterCode.git
```
### Test locally

To run the unit tests:
```
 $ chef exec rspec
```

Running integration tests and closing machine:
```
$ kitchen test
```

### Test in AWS

Running integration tests in AWS:
```
$ KITCHEN_YAML=kitchen_cloud.yml kitchen test
```
