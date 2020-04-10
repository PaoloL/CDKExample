# CDK Example  Templates

## Cloud Development Kits

All CDK developers need to install [Node.js](https://nodejs.org/en/download/) (>= 10.3.0)

You must specify your credentials and an AWS Region to use the AWS CDK CLI. The CDK looks for credentials and region in the following order:
- Using the `--profile` option to cdk commands.
- Using environment variables.
- Using the default profile as set by the AWS Command Line Interface (AWS CLI).

### Setup for Python

Other prerequisites depend on your development language, as follows.
- Python >= 3.6

Install the AWS CDK using the following command `npm install -g aws-cdk`

Setting Python virtualenv
- `cd CloudDevelopmentKit`
- `python3 -m venv myenv3`
- `source myenv3/bin/activate`

Updating Your Language Dependencies `pip install --upgrade aws-cdk.core`

To initialize your environment, you use the the following command
- `source .env/bin/activate`
- `pip install -r requirements.txt`
- `pip install aws_cdk.aws_ec2`

Adds multi profile/account and mfa support to cdk apps

Install [cdk-multi-profile-plugin](https://github.com/hupe1980/cdk-multi-profile-plugin/blob/master/cdk-multi-profile-plugin/README.md) with command `npm install cdk-multi-profile-plugin`

Synthesize an AWS CloudFormation template for the app `cdk synth`

Before you deploy the updated app, evaluate the difference between the AWS CDK app and the deployed app `cdk diff`

Deploy the stack, as follows `cdk deploy`

Destroy the app's resources to avoid incurring any costs `cdk destroy`

## Useful commands
`cdk ls` list all stacks in the app
`cdk synth` emits the synthesized CloudFormation template
`cdk deploy` deploy this stack to your default AWS account/region
`cdk diff` compare deployed stack with current state
`cdk docs` open CDK documentation
