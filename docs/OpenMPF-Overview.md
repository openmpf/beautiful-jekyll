> **NOTICE:** This software (or technical data) was produced for the U.S. Government under contract, and is subject to the Rights in Data-General Clause 52.227-14, Alt. IV (DEC 2007). Copyright 2016 The MITRE Corporation. All Rights Reserved.

# Overview

There are numerous video and image exploitation capabilities available today. The Open Media Processing Framework (OpenMPF) provides a framework for chaining, combining, or replacing individual components for the purpose of experimentation and comparison.

OpenMPF is a non-proprietary, scalable framework that permits practitioners and researchers to construct video, imagery, and audio exploitation capabilities using the available third-party components. Using OpenMPF, one can extract targeted entities in large-scale data environments, such as face and object detection.

For those developing new exploitation capabilities, OpenMPF exposes a set of Application Program Interfaces (APIs) for extending media analytics functionality. The APIs allow integrators to introduce new algorithms capable of detecting new targeted entity types. For example, a backpack detection algorithm could be integrated into an OpenMPF instance. OpenMPF does not restrict the number of algorithms that can operate on a given media file, permitting researchers, practitioners, and developers to explore arbitrarily complex composites of exploitation algorithms.

A list of open source algorithms currently integrated into the OpenMPF as distributed processing components is shown here:

| **Operation** | **Object Type** | **Framework**
|  --- | --- | ---
| Detection/Tracking | Face | OpenCV
| Detection/Tracking | Face | Dlib
| Detection/Tracking | Text | OpenALPR
| Detection/Tracking | Motion | OpenCV w/ STRUCT
| Detection/Tracking | Person | OpenCV
| Detection | Speech | Sphinx
| Detection| Classification | Caffe

The OpenMPF exposes data processing and job management web services via a User Interface (UI). These services allow users to upload media, create media processing jobs, determine the status of jobs, and retrieve the artifacts associated with completed jobs. The web services give application developers flexibility to use the OpenMPF in their preferred environment and programming language.