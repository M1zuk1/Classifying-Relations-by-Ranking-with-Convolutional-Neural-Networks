# Classifying-Relations-by-Ranking-with-Convolutional-Neural-Networks
Implementation of [Classifying Relations by Ranking with Convolutional Neural Networks](https://www.aclweb.org/anthology/P15-1061.pdf).


## Environment Requirements
* python 3.8
* pytorch 1.12.1

## Data
* [SemEval2010 Task8](https://drive.google.com/file/d/0B_jQiLugGTAkMDQ5ZjZiMTUtMzQ1Yy00YWNmLWJlZDYtOWY1ZDMwY2U4YjFk/view?sort=name&layout=list&num=50) \[[paper](https://www.aclweb.org/anthology/S10-1006.pdf)\]
* [glove.6B.300d.txt](https://nlp.stanford.edu/projects/glove/)

## Usage
1. Download the embedding and decompress it into the `embedding` folder.
2. Run the following the commands to start the program.
```shell
python run.py
```

3. You can use the official scorer to check the final predicted result.
```shell
perl semeval2010_task8_scorer-v1.2.pl proposed_answer.txt predicted_result.txt >> result.txt
```

## Result
The result of my version and that in paper are present as follows:
| paper | my version |
| :------: | :------: |
| 0.841 | 0.8364 |

The training log can be seen in `train.log` and the official evaluation results is available in `result.txt`.
