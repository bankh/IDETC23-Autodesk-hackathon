<div align="center" style="font-size: 22pt;"> 
    <strong>2023 IDETC Hackathon <br/> Automating Material Selection for Product Design</strong>  
</div>
<br/>
<div align="center">
    <img src="overview.png" width="500"/>
</div>
  
<br/>
Welcome to the Autodesk problem statement for the 2023 IDETC hackathon!
<br/>
<br/>

<div align="center">
  <strong>Material Category Definition Table</strong>
  <table border="1" style="width: 100%; text-align: center; margin: auto;">
    <thead>
        <tr>
            <th><strong>Material Category</strong></th>
            <th>Definition</th>
            <th>Example(s)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Metal_Aluminum</td>
            <td>Aluminum-based metal</td>
            <td>Aluminum alloy</td>
        </tr>
        <tr>
            <td>Metal_Ferrous</td>
            <td>Ferrous metal (excluding carbon steel)</td>
            <td>Cast iron</td>
        </tr>
        <tr>
            <td>Metal_Ferrous_Steel</td>
            <td>Carbon steel</td>
            <td>Stainless steel</td>
        </tr>
        <tr>
            <td>Metal_Non-Ferrous</td>
            <td>Non-Ferrous metal</td>
            <td>Platinum, silver</td>
        </tr>
        <tr>
            <td>Other</td>
            <td>Uncategorized material</td>
            <td>Glass, fabric, ceramic</td>
        </tr>
        <tr>
            <td>Plastic</td>
            <td>Plastic</td>
            <td>Thermoplastic</td>
        </tr>
        <tr>
            <td>Wood</td>
            <td>Natural and engineered wood</td>
            <td>Softwood</td>
        </tr>
    </tbody>
</table>


</div>
  
## Problem Statement
- The hackathon's goal is to predict the `material_category` for each body in the [test set](dataset/test_data). The [train data](dataset) contains material category labels for each body of each assembly in the `assembly.json` files.
- Link to [PDF](Autodesk%20Hackathon%20Problem%20Statement%202023.pdf) with more information.


## Dataset
- [Download instructions](dataset). Please note that the dataset has been modified for this hackathon, and you should only use data from these download instructions in your implementation.
  - The data has been modified to include in each `assembly.json` file a `material_category` label for each body. This label, which describes the material category of the body as defined in the table above, can be used to train your model.
- **Dataset Specifications:** Please refer to [the original documentation](https://github.com/AutodeskAILab/Fusion360GalleryDataset/blob/master/docs/assembly.md) of the Fusion 360 Gallery Dataset for information about the structure of the data in `assembly.json` and to find out more about the features in the dataset.

## Baseline 
- A GPT-based baseline can be found [here](baseline/gpt_baseline.ipynb).
- This can serve as an example of how to extract useful features from the data, and how to evaluate the method.

## Submission
- [Submission instructions](submission).

## References  
- [Bian, Shijie, et al. "Material prediction for design automation using graph representation learning." International Design Engineering Technical Conferences and Computers and Information in Engineering Conference. Vol. 86229. American Society of Mechanical Engineers, 2022.](https://arxiv.org/pdf/2209.12793.pdf)
>- [GitHub Repository](https://github.com/danielegrandi-adsk/material-gnn#material-prediction-for-design-automation-using-graph-representation-learning) of "Material prediction for design automation using graph representation learning."

