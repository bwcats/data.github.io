
<!DOCTYPE html>
<head>
    <meta charset="UTF-8">
    <title>药物分子表示数据库</title>
    <style>
        /* 设置表格的基本样式 */
        table {
            width: 100%;
            border-collapse: collapse;
        }
        td, th {
            border: 1px solid #ddd; /* 单元格边框 */
            padding: 8px; /* 单元格内边距 */
            text-align: center; /* 文本居中对齐 */
        }
 caption {
            font-size: 48px; /* 增大字体大小 */
            font-weight: bold; /* 加粗字体 */
            padding: 10px; /* 添加一些内边距 */
            caption-side: top; /* 将标题放置在表格的顶部 */
            text-align: center; /* 居中标题文本 */
        }

        /* 为第一列和第一行设置蓝色背景 */
        .first-col, .first-row {
            background-color: #3CA9B6;
            color: white; /* 设置文本颜色为白色 */
        }

        /* 为偶数行设置灰色背景，除了第一列 */
        tr:nth-child(even):not(:first-child)  {
            background-color: #E8F1F3; /* 背景 */
        }

        /* 为奇数行设置白色背景，除了第一行和第一列 */
        tr:nth-child(odd):not(:first-child) {
            background-color: #CEE2E5;
        }
    </style>
</head>

<body>
   <table>
   <caption>药物分子表示数据库</caption>
        <tr class="first-row">
           <th class="first-col">
             <td>数据集</td>
             <td>数据数量</td>
             <td>数据特征</td>
             <td>用途</td>
             <td>相关文献</td>
             <td>数据下载</td>
        </tr>
    <tr>
         <td class="first-col" rowspan="7">分类识别  </td>
          <tr>
      <td><br><a href = "https://moleculenet.org/datasets-1"><strong>ClinTox</strong></a></td>
      <td><br>1491</td>
      <td><br>已知化学结构的药物化合物临床试验毒性（或无毒性）和FDA 批准状态两个分类任务</td>
      <td><br>比较FDA 批准的药物和因毒性原因而未通过临床试验的药物<br></td>
      <td><a href = "https://pubs.rsc.org/en/content/articlehtml/2018/sc/c7sc02664a"><strong>MoleculeNet: a benchmark for molecular machine learning.2018</strong></a></td>
      <td><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/clintox.csv.gz"><strong>clintox.csv.gz</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "https://drugdesigndata.org/about/grand-challenge-4/bace"><strong>BACE</strong></a></td>
            </td>
      <td><br>1522</td>
      <td><br>人类β-分泌酶1(BACE-1)抑制剂数据库</td>
      <td>支持针对阿尔茨海默病和其他相关疾病的新药发现和开发过程</td>
      <td><br><a href = "https://pmc.ncbi.nlm.nih.gov/articles/PMC2879048/"><strong>The β-Secretase Enzyme BACE in Health and Alzheimer's Disease: Regulation, Cell Biology, Function, and Therapeutic Potential.2009</strong></a>
<br><br><a href = "https://pubs.acs.org/doi/abs/10.1021/acs.jmedchem.7b00393"><strong>BACE-1 Inhibitors: From Recent Single-Target Molecules to Multitarget Compounds for Alzheimer’s Disease.2017</strong></a>
<br><br><a href = "https://pubs.acs.org/doi/abs/10.1021/jm060154a"><strong>Structure-Based Design and Synthesis of Macroheterocyclic Peptidomimetic Inhibitors of the Aspartic Protease β-Site Amyloid Precursor Protein Cleaving Enzyme (BACE).2006</strong></a>
<br><br><a href = "https://www.sciencedirect.com/science/article/abs/pii/S0960894X09000729?via%3Dihub"><strong>Macrocyclic peptidomimetic β-secretase (BACE-1) inhibitors with activity in vivo.2009</strong></a>
</td>
      <td><br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=188"><strong>1146_data_598382.zip</strong></a>
<br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=220"><strong>GC4_Stage1a_participant_files.zip</strong></a>
<br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=222"><strong>GC4_BACE1_stage1_affinity.zip</strong></a>
<br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=211"><strong>1470_data_933024.gz</strong></a>
<br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=219"><strong>GC4_Stage1b_participant_files.zip</strong></a>
<br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=212"><strong>GC4_pose_release.tar.gz</strong></a>
<br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=215"><strong>BACE_score_compounds_D3R_GC4_answers.csv</strong></a>
<br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=216"><strong>BACE_FEset_compounds_D3R_GC4_answers.csv</strong></a>
<br><a href = "https://drugdesigndata.org/php/file-download.php?type=extended&id=223"><strong>GC4_BACE1_stage2_affinity.zip</strong></a>
</td>
    </tr>
    <tr>
      <td><br><a href = "https://moleculenet.org/"><strong>BBBP</strong></a></td>
      <td><br>超2000</td>
      <td><br>化合物的二元标签和血脑屏障穿透性数据</td>
      <td>预测血脑屏障的渗透性</td>
      <td><a href = "https://pmc.ncbi.nlm.nih.gov/articles/PMC8708321/"><strong>Prediction of Blood-Brain Barrier Penetration (BBBP) Based on Molecular Descriptors of the Free-Form and In-Blood-Form Datasets.2021</strong></a></td>
      <td><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/BBBP.csv"><strong>BBBP.csv</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "http://sideeffects.embl.de/"><strong>SIDER</strong></a></td>
      <td><br>1454</td>
      <td>药物和系统器官类别的副作用信息、上市药物及其副作用信息</td>
      <td>预测药物的副作用</td>
      <td><br><a href = "http://www.ncbi.nlm.nih.gov/pubmed/26481350"><strong>The SIDER database of drugs and side effects.2016</strong></a>
              <br><br><a href = "http://www.ncbi.nlm.nih.gov/pubmed/20087340"><strong>A side effect resource to capture phenotypic effects of drugs.2009</strong></a></td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/sider.csv.gz"><strong>sider.csv.gz</strong></a></td>
    </tr>
    <tr>
       <td><br><a href = "https://moleculenet.org/datasets-1"><strong>Tox21</strong></a></td>
      <td><br>8014</td>
      <td>化合物的不同毒性测量数据</td>
      <td>预测化学物质引起的生物毒性</td>
      <td><br><a href = "https://www.sciencedirect.com/science/article/abs/pii/S0378427417304125?via%3Dihub"><strong>DeepTox: Toxicity prediction using deep learning.2017</strong></a></td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/tox21.csv.gz"><strong>tox21.csv.gz</strong></a></td>
    </tr>
<tr>
<td><br><a href = "https://moleculenet.org/datasets-1"><strong>MUV</strong></a></td>
      <td><br>约90,000</td>
      <td>基准数据集</td>
      <td>验证虚拟筛选技术</td>
      <td><br><a href = "https://academic.oup.com/bib/article/22/4/bbaa266/5955940?login=false"><strong>TrimNet: learning molecular representation from triplet messages for biomedicine.2020</strong></a> </td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/muv.csv.gz"><strong>muv.csv.gz</strong></a> </td>
    </tr>
    </tr>

    <tr>
         <td class="first-col" rowspan="12">分类识别  </td>
    <tr>
       <td><br><a href = "http://quantum-machine.org/datasets/"><strong>QM7</strong></a></td>
      <td><br>7165</td>
      <td>GDB-13数据库的一个子集，每个分子最多包含23个原子</td>
      <td>预测分子的量子化学特性</td>
      <td><br><a href = "http://dx.doi.org/10.1021/ja902302h"><strong>970 Million Druglike Small Molecules for Virtual Screening in the Chemical Universe Database GDB-13.2009</strong></a>
<br><br><a href = "http://dx.doi.org/10.1103/PhysRevLett.108.058301"><strong>Fast and Accurate Modeling of Molecular Atomization Energies with Machine Learning.2012</strong></a></td>
      <td><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/qm7.mat"><strong>qm7.mat</strong></a></td>
    </tr>
    <tr>
<td><br><a href = "https://moleculenet.org/datasets-1"><strong>QM8</strong></a></td>
      <td><br>21758</td>
      <td>有机分子的量子化学属性，分子最多包含8个重原子，QM7数据集的扩展</td>
      <td>预测分子的量子化学特性</td>
      <td><br><a href = "http://scitation.aip.org/content/aip/journal/jcp/143/8/10.1063/1.4928757"><strong>Electronic spectra from TDDFT and machine learning in chemical space .2015</strong></a> 
<br><br><a href = "http://pubs.acs.org/doi/abs/10.1021/ci300415d"><strong>Enumeration of 166 Billion Organic Small Molecules in the Chemical Universe Database GDB-17.2012</strong></a></td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/qm8.csv"><strong>qm8.csv</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "https://moleculenet.org/datasets-1"><strong>QM9</strong></a></td>
      <td><br>约130,000</td>
      <td>分子的几何、能量、电子和热力学属性、完整空间信息，并提供原子特征</td>
      <td>预测分子的量子化学特性</td>
      <td><br><a href = "http://pubs.acs.org/doi/abs/10.1021/ci300415d"><strong>Enumeration of 166 Billion Organic Small Molecules in the Chemical Universe Database GDB-17.2012</strong></a>
<br><br><a href = "http://www.nature.com/articles/sdata201422"><strong>Quantum chemistry structures and properties of 134 kilo molecules.2014</strong></a></td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/qm9.csv"><strong>qm9.csv</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "https://moleculenet.org/datasets-1"><strong>ESOL</strong></a></td>
      <td><br>1128</td>
      <td>化合物的结构和水溶解度数据</td>
      <td>验证机器学习模型从分子结构直接估算溶解度的能力</td>
      <td><br><a href = "https://paperswithcode.com/paper/an-adaptive-graph-learning-method-for"><strong>An adaptive graph learning method for automated molecular interactions and properties predictions.2022</strong></a></td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/delaney-processed.csv"><strong>delaney-processed.csv</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "https://moleculenet.org/datasets-1"><strong>FreeSolv</strong></a></td>
      <td><br>643</td>
      <td><br>分子SMILES字符串和PubChem化合物ID</td>
      <td>预测水合作用的自由能变化</td>
      <td><br><a href = "http://dx.doi.org/10.1007/s10822-014-9747-x"><strong>FreeSolv: a database of experimental and calculated hydration free energies, with input files.2014</strong></a></td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/SAMPL.csv"><strong>SAMPL.csv</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "https://moleculenet.org/datasets-1"><strong>Lipophilicity</strong></a></td>
      <td><br>4200</td>
      <td>化合物在pH 7.4下的辛醇/水分配系数(logD)的实验结果</td>
      <td>预测化合物的辛醇/水分配系数(logD)</td>
      <td><br><a href = "https://analyticalsciencejournals.onlinelibrary.wiley.com/doi/abs/10.1002/cem.2718"><strong>In silico evaluation of logD7.4 and comparison with other prediction methods.2015</strong></a></td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/Lipophilicity.csv"><strong>Lipophilicity.csv</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "https://drugdesign.unistra.fr/LIT-PCBA/page2.htm"><strong>PCBA</strong></a></td>
      <td><br>超400,000</td>
      <td>通过高通量筛选生成的分子生物活性数据，化合物的多个生物活性测试</td>
      <td>识别潜在的药物候选分子</td>
      <td><br><a href = "https://pubs.acs.org/doi/abs/10.1021/acs.jcim.0c00155"><strong>LIT-PCBA: An Unbiased Data Set for Machine Learning and Virtual Screening.2020</strong></a></td>
      <td></td>
    </tr>
    <tr>
      <td><br><a href = "https://moleculenet.org/datasets-1"><strong>HIV</strong></a></td>
      <td><br>超40,000</td>
      <td>化合物的HIV抑制活性数据</td>
      <td>预测新类别的HIV抑制剂</td>
      <td><br><a href = "https://link.springer.com/chapter/10.1007/978-3-540-89689-0_33"><strong>IAM Graph Database Repository for Graph Based Pattern Recognition and Machine Learning.2008</strong></a></td>
      <td><br><a href = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/HIV.csv"><strong>HIV.csv</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "http://pdbbind.org.cn/"><strong>PDBbind</strong></a></td>
      <td><br>23,496</td>
      <td>蛋白质-配体复合物的实验结合亲和力数据,提供详细3D坐标</td>
      <td>阐述蛋白质如何与小分子（如药物）相互作用，推动药物设计和结构生物学研究</td>
      <td><br><br><a href = "https://pubs.acs.org/doi/10.1021/acs.jcim.8b00545"><strong>Comparative Assessment of Scoring Functions: The CASF-2016 Update.2018</strong></a>
<br><br><a href = "https://www.nature.com/articles/nprot.2017.114"><strong>Assessing protein–ligand interaction scoring functions with the CASF-2013 benchmark.2017</strong></a>
<br><br><a href = "http://pubs.acs.org/doi/abs/10.1021/acs.accounts.6b00491"><strong>Forging the Basis for Developing Protein–Ligand Interaction Scoring Functions.2017</strong></a>
<br><br><a href = "http://bioinformatics.oxfordjournals.org/content/31/3/405.long"><strong>PDB-wide collection of binding data: current status of the PDBbind database.2014</strong></a>
<br><br><a href = "http://pubs.acs.org/doi/abs/10.1021/ci500080q"><strong>Comparative Assessment of Scoring Functions on an Updated Benchmark: 1. Compilation of the Test Set.2014</strong></a>
<br><br><a href = "https://pubs.acs.org/doi/abs/10.1021/ci500081m"><strong>Comparative Assessment of Scoring Functions on an Updated Benchmark: 2. Evaluation Methods and General Results.2014</strong></a>
<br><br><a href = "http://pubs.acs.org/doi/abs/10.1021/ci9000053"><strong>Comparative Assessment of Scoring Functions on a Diverse Test Set.2009</strong></a>
      <td></td>
    </tr>
    <tr>
      <td><br><a href = "https://zinc15.docking.org/"><strong>ZINC</strong></a></td>
      <td><br>约250,000</td>
      <td>分子图，最多包含38个重原子</td>
      <td><br>计算回归水-辛醇分配系数（logP）减去合成可接受性（SAS）和环的数量</td>
      <td><br><a href = "http://pubs.acs.org/doi/abs/10.1021/acs.jcim.5b00559"><strong>ZINC 15 – Ligand Discovery for Everyone.2015</strong></a></td>
      <td><br><a href = "https://zinc15.docking.org/tranches/download"><strong>ZINC-downloader-2D-txt.uri</strong></a>
<br><a href = "https://zinc15.docking.org/tranches/download"><strong>ZINC-downloader-3D-db2.gz.uri</strong></a></td>
    </tr>
    <tr>
      <td><br><a href = "https://www.ebi.ac.uk/chembl/"><strong>ChEMBL</strong></a></td>
      <td><br>约324900</td>
      <td><br>集成化合物、药物、适应症、作用机制、靶点等，是生物活性数据的大型数据库</td>
      <td><br>药物发现和分子特性预测<br></td>
      <td><br><a href = "https://academic.oup.com/nar/article/doi/10.1093/nar/gkad1004/7337608"><strong>The ChEMBL Database in 2023: a drug discovery platform spanning multiple bioactivity data types and time periods.2023</strong></a>
<br><br><a href = "https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4489243/"><strong>ChEMBL web services: streamlining access to drug discovery data and utilities.2015</strong></a></td>
      <td><br><a href = "https://chembl.gitbook.io/chembl-interface-documentation/downloads"><strong>CHEMBL</strong></a></td>
    </tr>
   </tr>
  </table>
</body>
