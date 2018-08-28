---
swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 0
info:
  title: AWS Machine Learning API Predict
  version: 1.0.0
  description: Generates a prediction for the observation using the specified ML Model.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateBatchPrediction:
    get:
      summary: Create Batch Prediction
      description: Generates predictions for a group of observations.
      operationId: createBatchPrediction
      x-api-path-slug: actioncreatebatchprediction-get
      parameters:
      - in: query
        name: BatchPredictionDataSourceId
        description: The ID of the DataSource that points to the group of observations
          to predict
        type: string
      - in: query
        name: BatchPredictionId
        description: A user-supplied ID that uniquely identifies the                BatchPrediction
        type: string
      - in: query
        name: BatchPredictionName
        description: A user-supplied name or description of the BatchPrediction
        type: string
      - in: query
        name: MLModelId
        description: The ID of the MLModel that will generate predictions for the
          group of observations
        type: string
      - in: query
        name: OutputUri
        description: The location of an Amazon Simple Storage Service (Amazon S3)
          bucket or directory to store the batch prediction results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=Predict:
    get:
      summary: Predict
      description: Generates a prediction for the observation using the specified
        ML Model.
      operationId: predict
      x-api-path-slug: actionpredict-get
      parameters:
      - in: query
        name: MLModelId
        description: A unique identifier of the MLModel
        type: string
      - in: query
        name: PredictEndpoint
        description: 'Type: String'
        type: string
      - in: query
        name: Record
        description: A map of variable name-value pairs that represent an observation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Predict
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---