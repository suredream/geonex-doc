# GeoNEX-core Restful APIs Document
## 1. Start Runner

  - **Name**: Start RealTime Runner
  - **Description**: This api is used to start a real-timer runner in GEONEX dash
  - **Http Request Method**: GET
  - **URL**: [/start-runner](/start-runner)
  - **Input Parameter**:

  ```
  instance_type : String
  	image_name: String
  	s3_output: String
  	runner_id : String
  	runner_name : String
  ```

  - **Output Parameter**: success or error code
  - **Request Example**: [/start-runner?instance_type=m5d.4xlarge&image_name=geonex/active_fire_go16abi15:1.5&s3_output=s3://geonex/GO16_ABI15&runner_id=8dcdfcd4-c21a-c8ba-5152-9475dea5f1bd&runner_name=Production](/start-runner?instance_type=m5d.4xlarge&image_name=geonex/active_fire_go16abi15:1.5&s3_output=s3://geonex/GO16_ABI15&runner_id=8dcdfcd4-c21a-c8ba-5152-9475dea5f1bd&runner_name=Production)

## 2. Restart Runner

  - **Name**: Restart Runner
  - **Description**: This api is used to restart a real-timer runner in GEONEX dash
  - **Http Request Method**: GET
  - **URL**: /restart-runner
  - **Input Parameter**:

  ```
  instance_id : String
  	image_name: String
  	s3_output: String
  	runner_id : String
  	runner_name : String
  ```

  - **Output Parameter**: success or error code
  - **Request Example**: [/restart-runner?instance_id=i-01730beccb93d7c5c&image_name=geonex/active_fire_go16abi15:1.5&s3_output=s3://geonex/GO16_ABI15&runner_id=8dcdfcd4-c21a-c8ba-5152-9475dea5f1bd&runner_name=Production](/restart-runner?instance_id=i-01730beccb93d7c5c&image_name=geonex/active_fire_go16abi15:1.5&s3_output=s3://geonex/GO16_ABI15&runner_id=8dcdfcd4-c21a-c8ba-5152-9475dea5f1bd&runner_name=Production)

## 3. Stop Runner

  - **Name**: Stop Runner
  - **Description**: This api is used to stop a real-timer runner in GEONEX dash
  - **Http Request Method**: GET
  - **URL**: /stop-runner
  - **Input Parameter**:
  ```
  instance_id : String
  	runner_id : String
  	runner_name : String
  ```

  - **Output Parameter**: success or error code
  - **Request Example**: [/stop-runner?instance_id=i-01730beccb93d7c5c&runner_id=8dcdfcd4-c21a-c8ba-5152-9475dea5f1bd&runner_name=Production](/stop-runner?instance_id=i-01730beccb93d7c5c&runner_id=8dcdfcd4-c21a-c8ba-5152-9475dea5f1bd&runner_name=Production)

## 4. Delete Runner

  - **Name**: Delete Runner
  - **Description**: This api is used to delete a real-timer runner in GEONEX dash
  - **Http Request Method**: GET
  - **URL**: /delete-runner
  - **Input Parameter**:

  ```
  instance_id : String
  	runner_id : String
  	runner_name : String
  ```

  - **Output Parameter**: success or error code
  - **Request Example**: [/delete-runner?instance_id=i-01730beccb93d7c5c&runner_id=8dcdfcd4-c21a-c8ba-5152-9475dea5f1bd](/delete-runner?instance_id=i-01730beccb93d7c5c&runner_id=8dcdfcd4-c21a-c8ba-5152-9475dea5f1bd)

## 5. Send Email

  - **Name**: Send Email
  - **Description**: This api is used to send email to applicant who requests to register his/her algorithm dockers in GEONEX dash
  - **Http Request Method**: GET
  - **URL**: /send-email
  - **Input Parameter**:

  ```
  image_name: String
  	user_name : String
  	email : String
  ```

  - **Output Parameter**: success or error code
  - **Request Example:** [/send-email?image_name=i-01730beccb93d7c5c&user_name=user1&email=email@gmail.com](/send-email?image_name=i-01730beccb93d7c5c&user_name=user1&email=email@gmail.com)

## 6. Get S3 Usage

  - **Name**: Get S3 Usage
  - **Description**: This api is used to send email to get the usage of s3 output in GEONEX dash
  - **Http Request Method**: GET
  - **URL**: /get-s3-usage
  - **Input Parameter**: N/A
  - **Output Parameter**: json
  - **Request Example**: [](/get-s3-usage)

## 7. Describe Images

  - **Name**: Describe Images
  - **Description**: This api is used to describe all images registered in GEONEX dash
  - **Http Request Method**: GET
  - **URL**: /describe-images
  - **Input Parameter**: json
  - **Output Parameter**: success or error code
  - **Request Example**: [/describe-images](/describe-images)

## 8. Describe Containers

  - **Name**: Describe Containers
  - **Description**: This api is used to describe all containers in GEONEX dash, including running, finished containers.
  - **Http Request Method**: GET
  - **URL**: /describe-containers
  - **Input Parameter**: N/A
  - **Output Parameter**: json
  - **Request Example**: [/describe-containers](/describe-containers)

## 9. Describe Runner Containers

  - **Name**: Describe Runner Containers
  - **Description**: This api is used to describe runner’s containers in GEONEX dash, including running, finished containers.
  - **Http Request Method**: GET
  - **URL**: /describe-runner-containers
  - **Input Parameter**: N/A
  - **Output Parameter**: json
  - **Request Example**: [/describe-runner-containers](/describe-runner-containers)

## 10. Describe Users

  - **Name**: Describe Users
  - **Description**: This api is used to describe users in GEONEX dash.
  - **Http Request Method:** GET
  - **URL**: /describe-users
  - **Input Parameter**: N/A
  - **Output Parameter**: json
  - **Request Example**: [/describe-users](/describe-users)

## 11. Register User

   - **Name**: Register User
   - **Description**: This api is used to register user in GEONEX dash.
   - **Http Request Method**: POST
   - **URL**: /register-user
   - **Input Parameter**: 

   ```
   user_name : String
   	password: String
   	Display_name : String
   email : String
   ```
   
   - **Output Parameter**: json
   - **Request Example**: [/describe-users](/describe-users)