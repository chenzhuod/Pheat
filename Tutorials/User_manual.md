
# Query Workflow
## Step 1: Select Cell Type
  - Choose one or more cell populations from:
    + CD8+ T cells
    + CD4+ T cells
    + NKT cells
    + MAIT cells
    + γδ T cells
    + Proliferating T cells
    + Exhausted T cells
    + Treg cells
## Step 2: Choose Input Mode
  - Current supported mode:
    + Manual Input
## Step 3: Enter Gene Names
  - Input target genes in the Gene Input panel.
    + For **Single gene**: PDCD1
    + For **Multiple genes**: PDCD1,LAG3,TIGIT
  - Gene symbols should follow official HGNC nomenclature.
## Step 4: Select Tissue Source
  - Available tissue sources include:
    + Liver;
    + PBMC (for peripheral blood mononuclear cells)
## Step 5: Select Sub-cell Type
  - Users may further refine analysis by selecting specific T-cell subclusters. Examples:
    + Tex<sup>pre</sup>
    + Tex<sup>int</sup>
    + Tex<sup>term</sup>
    + nTreg
    + eTreg
## Step 6: Submit Query
  - Click **Submit**
  - Pheat will retrieve matching records and perform expression analysis.

# Output Results
  - Results are presented as:
    + **Data Tables** including: Disease type, Cell type, Gene name, Expression value.
    + **Scatter Plots** Visualization of expression distributions across: Diseases, Cell populations, Tissue origins.
