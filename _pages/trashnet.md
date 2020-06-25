---
layout: page
title: TrashNet
permalink: /trashnet/
---

TrashNet is a project that I worked on in collaboration with
[CleanRobotics](https://www.cleanrobotics.com) as part of
the AI Fellowship at Insight Data Science[^1], New York.

TrashNet takes a multi-pronged approach to identifying trash, building two classes of models. One of these(EfficientDet) is designed for throughput, enabling parallel inference. 
The other class of models, using the SSD MobileNet v2 architecture
is designed for edge devices, allowing you to do on-premise inference.

I also wrote a Streamlit app to help visualize the predictions
from the model, allowing you to inspect your model performance. As I've built TrashNet, this has been especially useful in letting me know what data my model needs more learning on. The webapp is on course to be deployed internally at CleanRobotics by end of August 2020.

For a writeup on the project, click [here](https://jsaurabh.dev/cv/object-detection/insight/2020/06/23/trashnet.html).

For info on setting up TrashNet and other tutorials, head to the documentation [here](https://trashbot.readthedocs.io/).


[^1]: A 7-week intensive fellowship where you work on a real world project. Find out more [here](https://insightfellows.com/ai).
