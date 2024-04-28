# NASA C-MAPSS Dataset

### Data Set: FD001

- Train trjectories: 100
- Test trajectories: 100
- Conditions: ONE (Sea Level)
- Fault Modes: ONE (HPC Degradation)

### Data Set: FD002

- Train trjectories: 260
- Test trajectories: 259
- Conditions: SIX
- Fault Modes: ONE (HPC Degradation)

### Data Set: FD003

- Train trjectories: 100
- Test trajectories: 100
- Conditions: ONE (Sea Level)
- Fault Modes: TWO (HPC Degradation, Fan Degradation)

### Data Set: FD004

- Train trjectories: 248
- Test trajectories: 249
- Conditions: SIX
- Fault Modes: TWO (HPC Degradation, Fan Degradation)

### Experimental Scenario

Data sets consists of multiple multivariate time series. Each data set is further divided into training and test subsets. Each time series is from a different engine i.e., the data can be considered to be from a fleet of engines of the same type. Each engine starts with different degrees of initial wear and manufacturing variation which is unknown to the user. This wear and variation is considered normal, i.e., it is not considered a fault condition. There are three operational settings that have a substantial effect on engine performance. These settings are also included in the data. The data is contaminated with sensor noise.

The engine is operating normally at the start of each time series, and develops a fault at some point during the series. In the training set, the fault grows in magnitude until system failure. In the test set, the time series ends some time prior to system failure. The objective of the competition is to predict the number of remaining operational cycles before failure in the test set, i.e., the number of operational cycles after the last cycle that the engine will continue to operate. Also provided a vector of true Remaining Useful Life (RUL) values for the test data.

The data are provided as a zip-compressed text file with 26 columns of numbers, separated by spaces. Each row is a snapshot of data taken during a single operational cycle, each column is a different variable. The columns correspond to:

1. Unit number
2. Time, in cycles
3. Operational Setting 1
4. Operational Setting 2
5. Operational Setting 3
6. Sensor Measurement 1
7. Sensor Measurement 2
8. ...
9. Sensor Measurement 26

## Citation

```
@inproceedings{nasa-cmapss,
  author={Saxena, Abhinav and Goebel, Kai and Simon, Don and Eklund, Neil},
  booktitle={2008 International Conference on Prognostics and Health Management},
  title={Damage propagation modeling for aircraft engine run-to-failure simulation},
  year={2008},
  volume={},
  number={},
  pages={1-9},
  doi={10.1109/PHM.2008.4711414}}

```
