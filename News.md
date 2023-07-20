
## News



<div align="center">
<table border="0">
    <table>
    <tr>
    <td>
      <h2> A plasmid identification tool was accepted for publication by Nucleic Acids Research! </h2>
      <p><b>Jun. 24, 2023</b></p>
      <p>Plasmids are mobile genetic elements that carry crucial accessory genes. Cataloging plasmids is a fundamental step in elucidating their role in promoting horizontal gene transfer between bacteria. To identify plasmid contigs from short-read assemblies, we developed a tool called PLASMe that utilizes the Transformer. PLASMe leverages the strengths of both alignment and learning-based methods. The alignment component in PLASMe facilitates the easy identification of closely related plasmids, while order-specific Transformer models predict diverged plasmids with accuracy. 
      The tool is available at <a href="https://github.com/HubertTang/PLASMe">PLASMe.</a> Check out the paper at <a href="https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkad578/7222081">PLASMe: a tool to identify PLASMid contigs from short-read assemblies using transformer</a></p>
    </td>   
  </tr>  
  </table>
  <table>
    <tr>
    <td>
      <h2> A plasmid host prediction tool was accepted for publication by Bioinformatics!</h2>
      <p><b>Apr. 19, 2023</b></p>
      <p> In this work, we construct a tool named HOTSPOT, aiming at predicting the host association of plasmids. By incorporating the state-of-the-art language model, Transformer, in each node’s taxon classifier, the top-down tree search achieves an accurate host taxonomy prediction for the input plasmid contigs. We rigorously tested HOTSPOT on multiple datasets and all experiments show that HOTSPOT outperforms other popular methods. The tool is available at <a href="https://academic.oup.com/bioinformatics/article/39/5/btad283/7136643">HOTSPOT</a> Check out the paper at <a href="https://academic.oup.com/bioinformatics/article/39/5/btad283/7136643">HOTSPOT: hierarchical host prediction for assembled plasmid contigs with transformer</a></p>     
    </td>   
  </tr>  
  </table> 
  <table>
    <tr>
    <td>
      <h2> A new integrated software named PhaBOX for phage identification and analysis has been developed! </h2>
      <p><b>Jan. 3rd, 2023</b></p>
      <p> Bacteriophages (phages) play key roles in regulating the composition/function of the microbiome by infecting their host bacteria. Lacking integrated software for phage identification and analysis, novel phages awaiting to be discovered constitute a large portion of “viral dark matter”. In this work, we developed a web server, named PhaBOX, to accurately identify and analyze phage contigs in metagenomic data. To our best knowledge, this is the first web server for comprehensive phage contig analysis in metagenomic data. PhaBOX integrates our previously published tools: PhaMer, PhaTYP, PhaGCN, and CHERRY, for phage identification, lifestyle prediction, taxonomy classification, and host prediction, respectively. To help users conduct downstream analysis, PhaBOX also provides visualization of the essential features for making the predictions, such as the similarity-based relationships between the contigs and other phages, predicted proteins on the contigs, and protein homology. All the predictions and intermediate results are provided for users. We hope that it can help advance the field of phage study in various ecosystems. </p>
      <p>
        To try PhaBOX, please click the link <a href="https://phage.ee.cityu.edu.hk/">PhaBOX</a> 
      </p>
    </td>   
  </tr>  
  </table>
  <table>
    <tr>
    <td>
      <h2> A review on phage taxonomy classification was accepted for publication by Frontiers in Microbiology. </h2>
      <p><b>Dec. 22rd, 2022</b></p>
      <p> This is the first review conducted under the new ICTV classification framework since several large families were removed from ICTV in August 2022. This study provides a comprehensive review of phage classification in different scenarios and a practical guidance for choosing appropriate taxonomic classification pipelines.</p>
      <p>Paper: <a href="https://www.frontiersin.org/articles/10.3389/fmicb.2022.1032186">HaploDMF: viral haplotype reconstruction from long reads via deep matrix factorization</a></p>
    </td>   
  </tr>  
  </table>
       <table>
    <tr>
    <td>
      <h2> A viral haplotype reconstruction pipline was published in Bioinformatics. </h2>
      <p><b>Oct. 21th, 2022</b></p>
      <p> This work developed a tool “HaploDMF” to reconstruct viral haplotypes from TGS data. Unlike existing tools that reconstruct haplotypes by checking the identity of overlap between reads, HaploDMF utilizes a deep matrix factorization model with an adapted loss function to automatically learn latent features from aligned reads. It is able to achieve highly robust performance on data with different properties while existing tools’ performance can be affected by the overlap size between reads. </p>
      <p>Paper: <a href="https://doi.org/10.1093/bioinformatics/btac708">HaploDMF: viral haplotype reconstruction from long reads via deep matrix factorization</a></p> 
      <p>Tool: <a href="https://github.com/dhcai21/HaploDMF">HaploDMF</a></p> 
    </td>   
  </tr>  
  </table>

<table>
    <tr>
    <td>
      <h2> A phage lifestyle prediction tool was published in Briefings in Bioinformatics</h2>
      <p><b>Oct. 17th, 2022</b></p>
      <p> Bacteriophages (or phages), which infect bacteria, have two distinct lifestyles: virulent and temperate. Predicting the lifestyle of phages helps decipher their interactions with their bacterial hosts, aiding phages’ applications in fields such as phage therapy. Because experimental methods for annotating the lifestyle of phages cannot keep pace with the fast accumulation of sequenced phages, computational method for predicting phages’ lifestyles has become an attractive alternative. Despite some promising results, computational lifestyle prediction remains difficult because of the limited known annotations and the sheer amount of sequenced phage contigs assembled from metagenomic data. In particular, most of the existing tools cannot precisely predict phages’ lifestyles for short contigs. In this work, we develop PhaTYP (Phage TYPe prediction tool) to improve the accuracy of lifestyle prediction on short contigs. We design two different training tasks, self-supervised and fine-tuning tasks, to overcome lifestyle prediction difficulties. We rigorously tested and compared PhaTYP with four state-of-the-art methods: DeePhage, PHACTS, PhagePred and BACPHLIP. The experimental results show that PhaTYP outperforms all these methods and achieves more stable performance on short contigs. In addition, we demonstrated the utility of PhaTYP for analyzing the phage lifestyle on human neonates’ gut data. This application shows that PhaTYP is a useful means for studying phages in metagenomic data and helps extend our understanding of microbial communities.</p>
      <p>Paper: <a href="https://doi.org/10.1093/bib/bbac487">PhaTYP: predicting the lifestyle for bacteriophages using BERT </a></p> 
      <p>Tool: <a href="https://github.com/KennthShang/PhaTYP">PhaMer</a></p> 
    </td>   
  </tr>  
  </table>

  <table>
    <tr>
    <td>
      <h2> An phage identification tool is published today in Briefings in Bioinformatics!</h2>
      <p><b>Jun 30, 2022</b></p>
      <p>
        In this work, we adopt the state-of-the-art language model, Transformer, to conduct contextual embedding for phage contigs. By constructing a protein-cluster vocabulary, we can feed both the protein composition and the proteins’ positions from each contig into the Transformer. The Transformer can learn the protein organization and associations using the self-attention mechanism and predicts the label for test contigs. We rigorously tested our developed tool named PhaMer on multiple datasets with increasing difficulty, including quality RefSeq genomes, short contigs, simulated metagenomic data, mock metagenomic data and the public IMG/VR dataset. All the experimental results show that PhaMer outperforms the state-of-the-art tools. In the real metagenomic data experiment, PhaMer improves the F1-score of phage detection by 27%.
      </p>
      <p>Paper: <a href="https://doi.org/10.1093/bib/bbac258">Accurate identification of bacteriophages from metagenomic data using Transformer</a></p> 
      <p>Tool: <a href="https://github.com/KennthShang/PhaMer">PhaMer</a></p> 
    </td>   
  </tr>  
  </table>

  <table>
    <tr>
    <td>
      <h2> An phage host prediction tool was published in Briefings in Bioinformatics!</h2>
      <p><b>May 22, 2022</b></p>
      <p>
        Prokaryotic viruses, which infect bacteria and archaea, are key players in microbial communities. Predicting the hosts of prokaryotic viruses helps decipher the dynamic relationship between microbes. Experimental methods for host prediction cannot keep pace with the fast accumulation of sequenced phages. Thus, there is a need for computational host prediction. Despite some promising results, computational host prediction remains a challenge because of the limited known interactions and the sheer amount of sequenced phages by high-throughput sequencing technologies. The state-of-the-art methods can only achieve 43% accuracy at the species level. In this work, we formulate host prediction as link prediction in a knowledge graph that integrates multiple protein and DNA-based sequence features. Our implementation named CHERRY can be applied to predict hosts for newly discovered viruses and to identify viruses infecting targeted bacteria. We demonstrated the utility of CHERRY for both applications and compared its performance with 11 popular host prediction methods. To our best knowledge, CHERRY has the highest accuracy in identifying virus–prokaryote interactions. It outperforms all the existing methods at the species level with an accuracy increase of 37%. In addition, CHERRY’s performance on short contigs is more stable than other tools.
      </p>
      <p>Paper: <a href="https://doi.org/10.1093/bib/bbac182">CHERRY: a Computational metHod for accuratE pRediction of virus–pRokarYotic interactions using a graph encoder–decoder model</a>
      </p> 
      <p>
        Tool: <a href="https://github.com/KennthShang/CHERRY">CHERRY</a>
      </p>
    </td>   
  </tr>  
  </table>

  <table>
  <tr>
    <td>
      <h2>An RNA virus taxonomy classification tool is published in Briefings in Bioinformatics</h2>
      <p><b>Feb. 7, 2022</b></p>
      <p>"RdRp-based sensitive taxonomic classification of RNA viruses for metagenomic data" is published today!</p>
      <p>
        With advances in library construction protocols and next-generation sequencing technologies, viral metagenomic sequencing has become the major source for novel virus discovery. Conducting taxonomic classification for metagenomic data is an important means to characterize the viral composition in the underlying samples. However, RNA viruses are abundant and highly diverse, jeopardizing the sensitivity of comparison-based classification methods. To improve the sensitivity of read-level taxonomic classification, we developed an RNA-dependent RNA polymerase (RdRp) gene-based read classification tool RdRpBin. It combines alignment-based strategy with machine learning models in order to fully exploit the sequence properties of RdRp. We tested our method and compared its performance with the state-of-the-art tools on the simulated and real sequencing data. RdRpBin competes favorably with all. In particular, when the query RNA viruses share low sequence similarity with the known viruses (⁠∼0.4), our tool can still maintain a higher F-score than the state-of-the-art tools. The experimental results on real data also showed that RdRpBin can classify more RNA viral reads with a relatively low false-positive rate. Thus, RdRpBin can be utilized to classify novel and diverged RNA viruses.
      </p>
      <p>Paper: <a href="https://doi.org/10.1093/bib/bbac011">RdRp-based sensitive taxonomic classification of RNA viruses for metagenomic data</a></p>     
      <p>Tool: <a href="https://github.com/HubertTang/RdRpBin">RdRpBin</a></p>     
      </p>
    </td>   
  </tr>
  </table> 

</div>

