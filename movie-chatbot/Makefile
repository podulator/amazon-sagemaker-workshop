export DEPLOYMENT_BUCKET_NAME ?= movie-chatbot-deployment

init: ##=> Install OS deps, python3.6 and dev tools
	$(info [*] Creating bucket... ${DEPLOYMENT_BUCKET_NAME})
	aws s3 ls | grep "${DEPLOYMENT_BUCKET_NAME}" || aws s3 mb 's3://${DEPLOYMENT_BUCKET_NAME}'

build:
	sam build 

package: build
	# Package Lambda function defined locally and upload to S3 as an artifact
	sam package \
			--output-template-file packaged.yaml \
			--s3-bucket ${DEPLOYMENT_BUCKET_NAME}

deploy: package
	# Deploy SAM template as a CloudFormation stack
	sam deploy \
			--template-file packaged.yaml \
			--stack-name movie-chatbot \
			--capabilities CAPABILITY_IAM 
  
