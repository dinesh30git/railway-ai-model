# Railway AI Model – Train Precedence Decision System

This repository contains a trained Decision Tree model developed to assist
railway section controllers in deciding train precedence when delays occur.

## Problem Statement
When one train is delayed at a junction, the system must decide which other
train should be allowed to proceed first based on priority and schedule.

## Input to Model
- Delayed train number (single input)

## Output from Model
- Train number that should be given priority to go first

## Dataset
- daily_schedule.csv  
  Contains train numbers, arrival times, and priority levels derived from
  real-world railway schedules.

## Model Used
- Decision Tree Classifier (scikit-learn)

## Files in This Repository
- trained_model.pkl : Trained decision tree model
- label_encoder.pkl : Encoder used for train labels
- daily_schedule.csv : Daily train schedule data
- README.md : Project documentation

## Usage
The model is intended to be loaded in a backend service (FastAPI / Flask).
The frontend sends the delayed train number, and the backend returns the
recommended train to proceed.

## Status
Model trained, tested, and ready for integration.
