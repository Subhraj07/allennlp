./bin/allennlp train tutorials/getting_started/simple_tagger.json --serialization-dir /tmp/tutorials/getting_started

```angular2html
{
  "training_duration": "00:28:28",
  "training_start_epoch": 0,
  "training_epochs": 36,
  "training_accuracy": 0.987103293953466,
  "training_accuracy3": 0.9986285219316186,
  "training_loss": 0.043649433851242064,
  "validation_accuracy": 0.9095547773886944,
  "validation_accuracy3": 0.9680340170085042,
  "validation_loss": 0.49565399558313433,
  "best_validation_accuracy": 0.9057028514257128,
  "best_validation_accuracy3": 0.9669334667333667,
  "best_validation_loss": 0.4536468997117012,
  "best_epoch": 26
}

```

./bin/allennlp evaluate /tmp/tutorials/getting_started/model.tar.gz https://allennlp.s3.amazonaws.com/datasets/getting-started/sentences.small.test

./bin/allennlp predict /tmp/tutorials/getting_started/model.tar.gz /home/subhra/PycharmProjects/allennlp/datasets/input.txt