# Univision---Workflow_Based_Agentic_Computer_Vision
SoC 2026 repository documenting concepts, exercises, and prototype development for the UniVision Workflow-Based Agentic Computer Vision project.

-------

# SoC Mid-Term Progress Report (Week 1 – Week 6)

## Student Information

**Project:** UniVision
**Submission Type:** Mid-Term Progress Report
**Reporting Period:** Week 1 – Week 6

---

# Introduction

This report summarizes the learning progress, practical exercises, conceptual understanding, and implementation-oriented activities completed during the first six weeks of the UniVision Summer of Code program.

The primary objective during this phase was to build strong foundations in computational thinking, Python programming, modern web technologies, API design, workflow systems, and introductory computer vision concepts. These topics collectively establish the groundwork required for developing intelligent real-time visual systems.

---

# Week 1 – Computational Thinking Foundations

## Topics Studied

* Variables and data representation
* Conditional statements
* Loops and iteration
* Functions
* Events and state management
* Pipelines and data flow
* Flowchart design
* Introduction to block-based programming

## Resources Explored

* Scratch
* Blockly Games
* CS50 Week 0
* Code.org Computer Science Fundamentals

## Exercises Performed

### Camera Alert Flowchart

Designed a simple logical workflow:

```text
Start
↓

Motion Detected?
├── Yes → Capture Frame → Analyze Frame
└── No  → Continue Monitoring
```

### Event-Driven Systems

Studied how events trigger system behavior and how state changes occur in response to inputs.

### Pipeline Thinking

Practiced decomposing large systems into smaller sequential stages.

Example:

Input → Processing → Decision → Output

## Key Learnings

Week 1 established an understanding that AI systems are composed of many small logical operations rather than a single intelligent model. Learning computational thinking improved the ability to reason about system behavior, execution order, and decision-making processes.

---

# Week 2 – Python Foundations

## Topics Studied

* Python syntax
* Indentation
* Functions
* Lists
* Dictionaries
* Type hints
* Testing concepts
* Data filtering

## Resources Used

* CS50 Python
* Python for Everybody
* Kaggle Python
* Exercism

## Exercises Completed

### Average Confidence Calculator

Implemented a function to compute the average confidence score from a list.

Example:

scores = [0.82,0.91,0.76]

Average = 0.83

---

### Detection Dictionary

Example structure:

{
"label":"person",
"confidence":0.92,
"box":[120,45,210,280]
}

---

### Threshold Filtering

Studied methods for removing detections below a specified confidence threshold.

### Testing

Explored the importance of writing tests before systems become complex.

---

## Key Learnings

Python demonstrated how concise code can be used to process structured information. Particular emphasis was placed on debugging through observation and printing intermediate values to better understand program execution.

---

# Week 3 – Web Fundamentals and React Thinking

## Topics Studied

* HTML
* CSS
* JavaScript
* TypeScript
* Components
* State Management
* Events
* React Concepts

## Resources Used

* MDN Web Docs
* React Learn
* TypeScript Handbook
* Scrimba React

---

## Exercises Completed

### Three Stage Dashboard Design

Dashboard Layout:

Input
↓

Detection
↓

Output

---

### UI State Diagram

Waiting
↓

Running
↓

Completed

or

Waiting
↓

Running
↓

Error

---

### Component Thinking

Studied reusable UI components and their role in scalable frontend applications.

---

## Key Learnings

This week introduced frontend engineering concepts and highlighted how state changes drive updates in interactive applications. Understanding components and state management provides a foundation for building future UniVision dashboards.

---

# Week 4 – APIs and JSON Contracts

## Topics Studied

* APIs
* HTTP Methods
* JSON
* Validation
* Status Codes
* Structured Responses

## Resources Used

* FastAPI Tutorial
* Pydantic Documentation
* MDN HTTP
* Postman Learning Center

---

## Exercises Completed

### API Contract Design

Request

{
"image":"sample.jpg"
}

Response

{
"status":"success",
"detections":[]
}

---

### Route Design

Designed example routes:

/health

/analyze

/results

---

### Validation

Studied methods to ensure predictable and reliable API behavior.

---

## Key Learnings

A major takeaway was understanding APIs as contracts between systems. Designing clear request and response schemas helps reduce ambiguity and improves interoperability between services.

---

# Week 5 – Blocks, Graphs and Workflow Systems

## Topics Studied

* Visual Programming
* Nodes
* Ports
* Connections
* Directed Graphs
* DAGs
* Topological Sorting
* Validation

## Resources Used

* Blockly Documentation
* React Flow
* VisuAlgo
* NetworkX

---

## Exercises Completed

### Image Processing Pipeline

Load Image
↓

Resize
↓

Grayscale
↓

Object Detection
↓

Save Result

---

### Block Definitions

Example:

Block:

Object Detector

Inputs:

Image

Outputs:

Detections

Configurations:

Confidence Threshold

Model Name

---

### Graph Validation

Studied how cycles create invalid workflows.

Example:

A → B → C

↑     ↓

└─────┘

Invalid because execution order cannot be determined.

---

## Key Learnings

This section provided insight into how visual AI systems can be represented as executable graphs. Understanding dependency management is essential for scalable workflow execution.

---

# Week 6 – Images as Arrays

## Topics Studied

* Pixels
* Channels
* Grayscale Images
* RGB Images
* Resizing
* Cropping
* Normalization

## Resources Used

* OpenCV Tutorials
* LearnOpenCV
* Kaggle Computer Vision
* Szeliski Computer Vision Book

---

## Exercises Completed

### Image Shape Inspection

Example:

Height = 720

Width = 1280

Channels = 3

---

### Color to Grayscale Conversion

Observed how grayscale conversion removes color information while preserving structural features.

---

### Resizing Images

Original

1920 × 1080

Resized

640 × 640

Studied possible distortion introduced during resizing.

---

### Cropping Regions of Interest

Explored methods to isolate relevant objects within an image before analysis.

---

## Key Learnings

Week 6 introduced the representation of images as numerical arrays. Understanding image structure is an important prerequisite for object detection, OCR, and future computer vision modules.

---

# Overall Reflection

The first six weeks focused heavily on developing strong conceptual foundations across multiple domains required for UniVision.

Major concepts understood include:

* Computational Thinking
* Pipeline Design
* Python Programming
* API Contracts
* State Management
* Graph Execution
* Image Representation
* Visual Workflow Systems

This phase significantly improved the ability to decompose complex systems into smaller modules, reason about data flow, and understand how modern AI vision platforms are architected.

---

# Next Steps

Planned topics for subsequent weeks include:

* Image Preprocessing
* Object Detection
* OCR
* Tracking
* WebSockets
* Real-Time Event Streaming
* Agentic AI
* Retrieval-Augmented Generation
* Evaluation and Safety Mechanisms

---

# References

* CS50
* Scratch
* Blockly
* Python for Everybody
* Kaggle Learn
* MDN Web Docs
* React Learn
* TypeScript Handbook
* FastAPI Documentation
* Pydantic Documentation
* OpenCV Tutorials
* LearnOpenCV
* VisuAlgo
* NetworkX Documentation

---
