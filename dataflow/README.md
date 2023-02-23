# Instruction

1)  Go To Cloud Shell
2)  gcloud init
3)  pip install 'apache-beam[gcp]'
4)   
```python
python -m attendance \
	--input gs://<your-input-bucket>/csv-files/input/dept_data.txt \
	--output gs://<your-output-bucket>/dflow/output/part \
	--runner DataflowRunner \
	--project <your-project-id> \
	--region <your-region-name> \
	--temp_location gs://<your-output-bucket>/temp/ 
```

Refer: [Apache beam WordCount example]( https://beam.apache.org/get-started/wordcount-example/)

Refer: [Dataflow Guides]( https://cloud.google.com/dataflow/docs/guides/setting-pipeline-options)

Refer: [Use custom containers pre-build]( https://cloud.google.com/dataflow/docs/guides/using-custom-containers#prebuild)

Refer: [If you want to specify a network]( https://cloud.google.com/dataflow/docs/guides/specifying-networks#python)
