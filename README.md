# Template Repo for Developing Trackable Live Demo for Web PubSub Service

> Only `demo-template` will be add to `Azure Web PubSub` repo.

## Requirements

### Coding

- [ ] Use `microsoftawps_` as hub name prefix
- [ ] [Integrate Google Analytics](docs/how-to-integrate-google-analytics.md) in live demo
- [ ] Google Analytics: [Reuse event](docs/how-to-integrate-google-analytics.md#custom-methods)
- [ ] Google Analytics: Only send actions triggered by visitors, or errors. NO customer content involves

### Deployment

- [ ] Deploy to AzureSignalR Demo subscription `62f51b53-9e7e-4673-8fcf-e312c82e113b`
- [ ] Resource group should be named start with `awps-live-demo-`

### Pull Request

- [ ] Contains [README](./demo-template/README.md)
- [ ] Contains [deploy.py](./demo-template/deploy/deploy.sh)


## How to Integrate Google Analytics in Demo

[doc](docs/how-to-integrate-google-analytics.md)

## How to Deploy to Azure

1. Use [script](./deploy/common/setup-resource-group.sh) to create a locked resource group with a web pubsub service.
2. deploy other services in this group.

## How to Create Pull Request to Azure/azure-webpubsub Repo

1. Create another branch to remove Google Analytics.
2. Rename `demo-template` to a good name.
3. copy and create a pull request to `live-demo` branch
4. remove `google analytics` in code, and create a pull request to `main` branch

