Code is for fine-tuning Alpaca and Llama2 from https://github.com/tatsu-lab/stanford_alpaca

1. Go to stanford_alpaca directory
2. Do: pip install -r requirements.txt 
3. pip install deepspeed
4. pip install accelerator
5. Run model_trainer.sh under the stanford_alpaca directory

Note:
a. In model_trainer.sh
		If you want to use alpaca: 
			--model_name_or_path "wxjiao/alpaca-7b"		

b. Don't change other setups except for
		i. --data_path ../../data/train/coi_2.json \
			this is where the train data is located (change the path if needed)

		ii. --output_dir ../../alpaca_models/coi2\
			this is where the model is stored (change the path if needed)