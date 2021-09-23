Codes and data for performance evaluation is avaiable at:
https://drive.google.com/file/d/1-4I_Kc8CmILgU4IjUG3Izf2jtLkErXyj/view?usp=sharing


The file 'SSLsdCodes.rar' inclues:


1.  ScaleSpaceDetection.m:
---takes the data from the folder 'IndvSclDtctRslts' as input, which are the line segment sets produced by the seed detectors at individual scales (prepared in advance);
---performs our proposed scale-space approach;
---saves the scale-space detection results in the folder 'DetectionRslts'.

2. ObjectiveEvaluation.m:
---takes the line segment detection results of each pair of seed and scale-space detectors from the folder 'DetectionRslts' as input;
---performs objective evaluation with a corrected version of the evaluation method developed by Cho et al;


3. SubjectiveEvaluation.m:
---takes detection results from the folder 'DetectionRslts' as input;
---produces figures to show a visual comparision of each pair of seed and scale-space detectors;
---saves the figures with .eps format in the folder 'SubjEvalOutput'.


4. In the folder 'EvalDataFuncs':
---includes YorkUrban-LineSegment dataset and functions for objective evaluation, provided by Cho et al https://github.com/NamgyuCho/Linelet-code-and-YorkUrban-LineSegment-DB;
---to cope with the bugs of Cho et al as mentioned in the paper, two of the evaluation functions ('evaluate_line_segment_region.m' and 'line_area_intersection.m') have been corrected by us.


5. The folder 'ScaleSpaceFuncs' includes the functions of our proposed scale-space approach.


6. The codes have been tested with matlab2016.


