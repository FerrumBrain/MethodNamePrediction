# MethodNamePrediction
* Download java repository, set path to folder_path, change mode to `create_dataset` (or use prepared dataset with two columns: method and name, divided into 3 parts: train, validation, test. Set paths to train_file_name, validate_file_name, test_file_name)
* Then you can just run notebook (you might want to change line `test_dataset = test_dataset.shuffle(seed=42)[:10]` if it takes too many memory)
* As for the changes of quality of predictions: we can see that not tuned model can't even understand format of data it should provide. It guesses randomly. Tuned model gives pretty precise answers with some deviations from correct answers, but it gives us correct form of function names
