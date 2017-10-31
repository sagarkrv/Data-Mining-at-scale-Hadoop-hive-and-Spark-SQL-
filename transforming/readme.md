Step 1: Download the .sql files into your current directory and execute the shell command

Step 2: Launch the below commands in your shell
/data/spark15/bin/spark-sql –master yarn-client –conf spark.ui.port=40445 –executor-memory 15g –hiveconf load_date=`date +%Y-%m-%d` –driver-memory 10g –queue default –num-executors 20 –conf spark.yarn.executor.memoryOverhead=4096 –queue Q1 -i ./hospital.sql

/data/spark15/bin/spark-sql –master yarn-client –conf spark.ui.port=40445 –executor-memory 15g –hiveconf load_date=`date +%Y-%m-%d` –driver-memory 10g –queue default –num-executors 20 –conf spark.yarn.executor.memoryOverhead=4096 –queue Q1 -i ./eff_care.sql


/data/spark15/bin/spark-sql –master yarn-client –conf spark.ui.port=40445 –executor-memory 15g –hiveconf load_date=`date +%Y-%m-%d` –driver-memory 10g –queue default –num-executors 20 –conf spark.yarn.executor.memoryOverhead=4096 –queue Q1 -i ./readmissions.sql


/data/spark15/bin/spark-sql –master yarn-client –conf spark.ui.port=40445 –executor-memory 15g –hiveconf load_date=`date +%Y-%m-%d` –driver-memory 10g –queue default –num-executors 20 –conf spark.yarn.executor.memoryOverhead=4096 –queue Q1 -i ./measures.sql


/data/spark15/bin/spark-sql –master yarn-client –conf spark.ui.port=40445 –executor-memory 15g –hiveconf load_date=`date +%Y-%m-%d` –driver-memory 10g –queue default –num-executors 20 –conf spark.yarn.executor.memoryOverhead=4096 –queue Q1 -i ./survey_responses.sql


These files have DDLs that create the necessary parquet tables
