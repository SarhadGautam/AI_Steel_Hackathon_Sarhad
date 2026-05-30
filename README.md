<div><h1>Defect Detection in Hot Rolling</h1></div>
<div>In Hot Rolling Mills, one specific defect (referred to here as the <I>Alpha defect</I>) is a critical quality challenge. This defect cannot be detected through the existing system because the coil remains under tension in the inspection zones. Since it is not possible to detect Alpha defects inline, current quality control relies on sample observations at the final stage, where only a certain percentage of the total coils produced are inspected. Additionally, manual inspection is <B>time-intensive</B>, whereas the manufacturing and supply chain processes operate under strict time constraints. Although the Alpha defect accounts for only a very small percentage of the total production volume, it can still lead to customer complaints and product downgrades.</div> <br/> <br/>
<div>
<p data-start="748" data-end="883">During hot rolling, each stage has different process parameters that can contribute to the formation of the defect. Therefore, all stages must be considered to effectively detect the formation of Alpha defects.</p>
<p data-start="748" data-end="883">Detect the occurrence of the Alpha defect during rolling to prevent customer complaints and reduce downgrades through proactive action.</p> <br/> <br/>
<p><strong>Dataset Description</strong></p>
<p class="font-claude-response-body break-words whitespace-normal leading-[1.7]">The dataset folder contains the following files:</p>
<div class="overflow-x-auto w-full px-2 mb-6">
<table style="border-collapse:collapse;border-width:1px" border="1"><tbody>

<tr>
<th class="text-text-100 border-b-0.5 border-border-300/60 py-2 pr-4 align-top font-bold" style="border-width:1px" scope="col">File</th>
<th class="text-text-100 border-b-0.5 border-border-300/60 py-2 pr-4 align-top font-bold" style="border-width:1px" scope="col">Dimensions</th>
</tr>
<tr>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">train.csv</td>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">1352 × 51</td>
</tr>
<tr>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">test.csv</td>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">339 × 50</td>
</tr>
<tr>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">sample_submission.csv</td>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">339 × 2</td>
</tr>

</tbody></table>
</div>
<p><strong>Variable Description</strong></p>
<div class="overflow-x-auto w-full px-2 mb-6">
<table style="border-collapse:collapse;border-width:1px" border="1"><tbody>

<tr>
<th class="text-text-100 border-b-0.5 border-border-300/60 py-2 pr-4 align-top font-bold" style="border-width:1px" scope="col">Column Name</th>
<th class="text-text-100 border-b-0.5 border-border-300/60 py-2 pr-4 align-top font-bold" style="border-width:1px" scope="col">Description</th>
</tr>
<tr>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">CoilID</td>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">Unique identifier for each coil</td>
</tr>
<tr>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">X1–X49</td>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">Process parameters across multiple stages</td>
</tr>
<tr>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">Y</td>
<td class="border-b-0.5 border-border-300/30 py-2 pr-4 align-top" style="border-width:1px">Target variable: Alpha defect occurrence (1 = Defect, 0 = No Defect)</td>
</tr>

</tbody></table>
</div>
<p><strong>Evaluation Metric</strong></p>
<p class="font-claude-response-body break-words whitespace-normal leading-[1.7]">A model which will have 0 false negative and less than 10% False positive will be accepted.</p>
<ul class="[li_&amp;]:mb-0 [li_&amp;]:mt-1 [li_&amp;]:gap-1 [&amp;:not(:last-child)_ul]:pb-1 [&amp;:not(:last-child)_ol]:pb-1 list-disc flex flex-col gap-1 pl-8 mb-3">
<li>Recall – 100%</li>
<li>Precision - &gt; 90%</li>
</ul>
<p><strong>Submission Criteria</strong></p>
<ul class="[li_&amp;]:mb-0 [li_&amp;]:mt-1 [li_&amp;]:gap-1 [&amp;:not(:last-child)_ul]:pb-1 [&amp;:not(:last-child)_ol]:pb-1 list-disc flex flex-col gap-1 pl-8 mb-3">
<li>The submission file must be submitted in .csv format only.</li>
<li>The size of this submission file must be <strong>339 × 2</strong>.</li>
<li>Ensure that your submission file contains:
<ul class="[li_&amp;]:mb-0 [li_&amp;]:mt-1 [li_&amp;]:gap-1 [&amp;:not(:last-child)_ul]:pb-1 [&amp;:not(:last-child)_ol]:pb-1 list-disc flex flex-col gap-1 pl-8 mb-3">
<li>Correct CoilID values as per the test file</li>
<li>Correct column names as provided in the sample_submission.csv file</li>
</ul>
</li>
</ul>
<p><strong>Instructions</strong></p>
<ul class="[li_&amp;]:mb-0 [li_&amp;]:mt-1 [li_&amp;]:gap-1 [&amp;:not(:last-child)_ul]:pb-1 [&amp;:not(:last-child)_ol]:pb-1 list-disc flex flex-col gap-1 pl-8 mb-3">
<li>Click <strong>Download dataset</strong> to download the dataset.</li>
<li>Solve the problem in your local environment.</li>
<li>Save the predictions in a .csv file named expected_submission.csv.</li>
<li>Click <strong>Upload File</strong> (under the Upload File section) to upload your prediction file (.csv).</li>
<li>Click <strong>Upload File</strong> (under the Upload Source Code section) to upload your .ipynb file along with any presentation file.</li>
<li>Add any instructions or comments in the <strong>Your Answer</strong> section.</li>
<li>Click <strong>Submit</strong>.</li>
</ul>
</div>
