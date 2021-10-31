# great-expectation-practice

Exploring Data Pipeline Test. Building scalable pipelines

Testing is an important part of any system/platform/pipeline. As a Data Engineer, testing my Data Pipeline is very important and tools like great expectation made it very easy.

## Using Great Expectation

`great_expectations init` -  is used to initialized an empty project to set up all required files to enable proper testing of each part of the system

`great_expectations datasource new` - this command will generate a new datasource which allow great_expectation to ensure proper connection and get the required datatype or data value from the source

`great_expectations suite scaffold filename` - the command will create a new suite, which will generate a new jupyter notebook file that we can edit and specify the different kind of test that we want on each data column and value.

`great_expectations suite edit filename` - the command is used to edit the test notebook

`great_expectations checkpoint new filename` - the command create a new file that is used to store the current status of the test we have written

`great_expectations checkpoint run filename` - the command execute the checkpoint to ensure nothing as changed and the pipeline works fine. This is especially useful if you have written some test before and you need to switch to another project.

`great_expectations docs build --site-name local_site` - the command will generate an html page that shows test documentation that we have written so far.

Learn more here:: [Great Expectation Documentation](https://docs.greatexpectations.io/docs/)
