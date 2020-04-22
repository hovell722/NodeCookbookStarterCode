# Node Cookbook

Description

## List of what installs
- NodeJs
- Nginx
- pm2 and npm

## Commands

### Test locally

Running my unit test:
```
chef exec rspec
```

Running integration tests and closing machine:
```
kitchen test
```

### Test in AWS

Running integration tests in AWS
```
KITCHEN_YAML=kitchen_cloud.yml kitchen test
```
