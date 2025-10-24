<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Complete DME Coding Hierarchy - All Layers You Need to Master</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            max-width: 1600px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f5f5f5;
            color: #333;
        }
        .hero-section {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px;
            border-radius: 12px;
            margin-bottom: 30px;
            text-align: center;
        }
        .hero-section h1 {
            margin: 0 0 15px 0;
            font-size: 2.5em;
        }
        .section {
            background: white;
            padding: 30px;
            margin: 20px 0;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }
        h1, h2, h3, h4 {
            color: #333;
        }
        h2 {
            border-bottom: 3px solid #2196F3;
            padding-bottom: 10px;
            margin-top: 0;
        }
        .layer-card {
            background: #f9f9f9;
            border-left: 5px solid #2196F3;
            padding: 20px;
            margin: 15px 0;
            border-radius: 5px;
        }
        .layer-1 { border-left-color: #e91e63; }
        .layer-2 { border-left-color: #9c27b0; }
        .layer-3 { border-left-color: #3f51b5; }
        .layer-4 { border-left-color: #2196f3; }
        .layer-5 { border-left-color: #00bcd4; }
        .layer-6 { border-left-color: #009688; }
        .layer-7 { border-left-color: #4caf50; }
        .layer-8 { border-left-color: #8bc34a; }
        .layer-9 { border-left-color: #ff9800; }
        .layer-10 { border-left-color: #ff5722; }
        
        .hierarchy-diagram {
            background: linear-gradient(to bottom, #f8f9fa, #e9ecef);
            padding: 30px;
            border-radius: 8px;
            margin: 20px 0;
        }
        .hierarchy-level {
            background: white;
            padding: 20px;
            margin: 10px 0;
            border-radius: 8px;
            border-left: 5px solid;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .arrow-down {
            text-align: center;
            font-size: 30px;
            color: #666;
            margin: 5px 0;
        }
        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin: 20px 0;
        }
        .grid-3 {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 20px;
            margin: 20px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
            font-size: 14px;
        }
        th {
            background-color: #2196F3;
            color: white;
            padding: 12px;
            text-align: left;
            font-weight: bold;
        }
        td {
            padding: 10px;
            border-bottom: 1px solid #ddd;
        }
        tr:nth-child(even) {
            background-color: #f9f9f9;
        }
        .code-tag {
            display: inline-block;
            padding: 4px 8px;
            border-radius: 4px;
            font-family: 'Courier New', monospace;
            font-weight: bold;
            margin: 2px;
            font-size: 0.9em;
        }
        .boc-tag { background-color: #BBDEFB; color: #1565C0; }
        .hcpcs-tag { background-color: #FFE0B2; color: #E65100; }
        .icd-tag { background-color: #E1BEE7; color: #6A1B9A; }
        .modifier-tag { background-color: #C8E6C9; color: #2E7D32; }
        .pos-tag { background-color: #FFF9C4; color: #F57F17; }
        
        .critical-box {
            background-color: #FFEBEE;
            padding: 20px;
            border-radius: 8px;
            border: 3px solid #F44336;
            margin: 20px 0;
        }
        .warning-box {
            background-color: #FFF3E0;
            padding: 20px;
            border-radius: 8px;
            border: 3px solid #FF9800;
            margin: 20px 0;
        }
        .success-box {
            background-color: #E8F5E9;
            padding: 20px;
            border-radius: 8px;
            border: 3px solid #4CAF50;
            margin: 20px 0;
        }
        .info-box {
            background-color: #E3F2FD;
            padding: 20px;
            border-radius: 8px;
            border: 3px solid #2196F3;
            margin: 20px 0;
        }
        .workflow-step {
            background: white;
            padding: 20px;
            border-radius: 8px;
            margin: 15px 0;
            border-left: 5px solid #4CAF50;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .workflow-step h4 {
            margin: 0 0 10px 0;
            color: #2E7D32;
        }
        .checklist {
            background-color: #FFF9C4;
            padding: 20px;
            border-radius: 8px;
            margin: 15px 0;
            border: 2px solid #FBC02D;
        }
        .checklist ul {
            margin: 10px 0;
            padding-left: 20px;
        }
        .checklist li {
            margin: 8px 0;
        }
        .expandable {
            background: #f5f5f5;
            border: 1px solid #ddd;
            border-radius: 5px;
            margin: 10px 0;
            overflow: hidden;
        }
        .expandable-header {
            background: #e0e0e0;
            padding: 15px;
            cursor: pointer;
            font-weight: bold;
            user-select: none;
            transition: background-color 0.2s ease;
        }
        .expandable-header:hover {
            background: #d5d5d5;
        }
        .expandable-header:active {
            background: #c0c0c0;
        }
        .expandable-content {
            padding: 15px;
            display: none;
        }
        ul, ol {
            margin: 10px 0;
            padding-left: 25px;
        }
        li {
            margin: 8px 0;
        }
        .highlight-yellow {
            background-color: #FFEB3B;
            padding: 2px 5px;
            border-radius: 3px;
        }
        .highlight-green {
            background-color: #C8E6C9;
            padding: 2px 5px;
            border-radius: 3px;
        }
        .highlight-red {
            background-color: #FFCDD2;
            padding: 2px 5px;
            border-radius: 3px;
        }
        @media print {
            body {
                background-color: white;
            }
            .section {
                box-shadow: none;
                page-break-inside: avoid;
            }
        }
    </style>
</head>
<body>

<div class="hero-section">
    <h1>🏥 THE COMPLETE DME CODING HIERARCHY</h1>
    <p style="font-size: 1.3em; margin: 10px 0;">Every Layer You Need to Master for DME Business Success</p>
    <p style="font-size: 1.1em; opacity: 0.9;">From BOC Licensing to Claims Payment - A Comprehensive Guide</p>
</div>

<!-- TABLE OF CONTENTS -->
<div class="section">
    <h2>📋 Table of Contents</h2>
    <ol>
        <li><a href="#10layers">The 10 Essential Layers of DME Coding</a></li>
        <li><a href="#layer1">Layer 1: BOC Licensing Foundation</a></li>
        <li><a href="#layer2">Layer 2: HCPCS Product Codes</a></li>
        <li><a href="#layer3">Layer 3: ICD-10 Medical Necessity</a></li>
        <li><a href="#layer4">Layer 4: Modifiers - The Critical Add-Ons</a></li>
        <li><a href="#layer5">Layer 5: Documentation Requirements</a></li>
        <li><a href="#layer6">Layer 6: LCD/NCD Coverage Determinations</a></li>
        <li><a href="#layer7">Layer 7: Prior Authorization</a></li>
        <li><a href="#layer8">Layer 8: Claims Submission Data</a></li>
        <li><a href="#layer9">Layer 9: Rental vs Purchase Classifications</a></li>
        <li><a href="#layer10">Layer 10: Payer-Specific Requirements</a></li>
        <li><a href="#workflow">Complete Claims Workflow</a></li>
        <li><a href="#boc-details">Your 36 BOC Codes in Detail</a></li>
        <li><a href="#common-errors">Common Errors to Avoid</a></li>
        <li><a href="#systems">Data Management Systems Needed</a></li>
    </ol>
</div>

<!-- 10 LAYERS OVERVIEW -->
<div class="section" id="10layers">
    <h2>🔟 The 10 Essential Layers of DME Coding</h2>
    
    <div class="info-box">
        <strong>Critical Understanding:</strong> Most DME suppliers fail because they think it's just about BOC + HCPCS + ICD-10. 
        In reality, there are <strong>10 interconnected layers</strong> of data you must collect, verify, and maintain for every single transaction.
        Missing any one layer = denied claim = lost revenue.
    </div>

    <div class="hierarchy-diagram">
        <div class="hierarchy-level layer-1" style="border-left-color: #e91e63;">
            <strong>LAYER 1: BOC LICENSING FOUNDATION</strong>
            <p>Your authorization to operate - 36 BOC categories defining what you can legally sell</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-2" style="border-left-color: #9c27b0;">
            <strong>LAYER 2: HCPCS PRODUCT CODES</strong>
            <p>Exact product identification - the "what" you're billing for</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-3" style="border-left-color: #3f51b5;">
            <strong>LAYER 3: ICD-10 MEDICAL NECESSITY</strong>
            <p>The "why" - proving the patient needs this equipment</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-4" style="border-left-color: #2196f3;">
            <strong>LAYER 4: MODIFIERS</strong>
            <p>Critical add-ons that change how the claim is processed (KX, GA, GY, etc.)</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-5" style="border-left-color: #00bcd4;">
            <strong>LAYER 5: DOCUMENTATION REQUIREMENTS</strong>
            <p>Prescriptions, CMN, face-to-face visits, physician notes</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-6" style="border-left-color: #009688;">
            <strong>LAYER 6: LCD/NCD COVERAGE DETERMINATIONS</strong>
            <p>Regional and national coverage policies that dictate payment</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-7" style="border-left-color: #4caf50;">
            <strong>LAYER 7: PRIOR AUTHORIZATION</strong>
            <p>Pre-approval required for certain items before delivery</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-8" style="border-left-color: #8bc34a;">
            <strong>LAYER 8: CLAIMS SUBMISSION DATA</strong>
            <p>NPI, Place of Service, dates, quantities, pricing</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-9" style="border-left-color: #ff9800;">
            <strong>LAYER 9: RENTAL VS PURCHASE CLASSIFICATION</strong>
            <p>Capped rental, recurring purchase, or one-time purchase rules</p>
        </div>
        <div class="arrow-down">⬇</div>
        
        <div class="hierarchy-level layer-10" style="border-left-color: #ff5722;">
            <strong>LAYER 10: PAYER-SPECIFIC REQUIREMENTS</strong>
            <p>Medicare vs Medicaid vs private insurance variations</p>
        </div>
    </div>
</div>

<!-- LAYER 1: BOC LICENSING -->
<div class="section" id="layer1">
    <h2>📜 LAYER 1: BOC Licensing Foundation</h2>
    
    <div class="layer-card layer-1">
        <h3>What is BOC Licensing?</h3>
        <p><strong>BOC (Business Operation Code)</strong> is your Medicare accreditation that authorizes you to sell specific categories of DME. 
        You currently have <strong>36 BOC categories</strong> licensed.</p>
        
        <div class="warning-box">
            <strong>⚠️ CRITICAL RULE:</strong> You can ONLY bill for items that fall under your licensed BOC categories. 
            Selling outside your BOC categories = Medicare fraud = potential loss of accreditation + fines.
        </div>
    </div>

    <h3>Your 36 BOC Categories:</h3>
    <div class="grid-3">
        <div>
            <h4 style="color: #2196F3;">Durable Medical Equipment (DM)</h4>
            <ul>
                <li><span class="code-tag boc-tag">DM02</span> Commodes</li>
                <li><span class="code-tag boc-tag">DM05</span> BGM (Non-Mail)</li>
                <li><span class="code-tag boc-tag">DM06</span> BGM (Mail Order)</li>
                <li><span class="code-tag boc-tag">DM08</span> Heat/Cold Apps</li>
                <li><span class="code-tag boc-tag">DM11</span> (Reserved)</li>
                <li><span class="code-tag boc-tag">DM12</span> Infusion Pumps</li>
                <li><span class="code-tag boc-tag">DM13</span> Insulin Pumps</li>
                <li><span class="code-tag boc-tag">DM14</span> Implanted Pumps</li>
                <li><span class="code-tag boc-tag">DM15</span> Lymphedema Pumps</li>
                <li><span class="code-tag boc-tag">DM16</span> Misc DME</li>
                <li><span class="code-tag boc-tag">DM17</span> Wound VAC</li>
                <li><span class="code-tag boc-tag">DM18</span> Bone Stimulators</li>
                <li><span class="code-tag boc-tag">DM20</span> (Reserved)</li>
                <li><span class="code-tag boc-tag">DM21</span> (Reserved)</li>
                <li><span class="code-tag boc-tag">DM22</span> (Reserved)</li>
                <li><span class="code-tag boc-tag">DM24</span> Pressure Mattresses</li>
                <li><span class="code-tag boc-tag">DM25</span> Support Surfaces</li>
                <li><span class="code-tag boc-tag">DM28</span> (Reserved)</li>
                <li><span class="code-tag boc-tag">DM29</span> (Reserved)</li>
            </ul>
        </div>
        <div>
            <h4 style="color: #FF9800;">Mobility & Other Categories</h4>
            <ul>
                <li><span class="code-tag boc-tag">M01</span> Canes</li>
                <li><span class="code-tag boc-tag">M05</span> Walkers</li>
                <li><span class="code-tag boc-tag">M06</span> Wheelchairs</li>
                <li><span class="code-tag boc-tag">M06A</span> Wheelchair Parts</li>
                <li><span class="code-tag boc-tag">M07</span> Pediatric Wheelchairs</li>
                <li><span class="code-tag boc-tag">M07A</span> Special Size Wheelchairs</li>
                <li><span class="code-tag boc-tag">M10</span> Walker Accessories</li>
                <li><span class="code-tag boc-tag">OR03</span> Custom Fabricated Orthotics</li>
                <li><span class="code-tag boc-tag">OR04</span> Custom Fitted Orthotics</li>
                <li><span class="code-tag boc-tag">PD04</span> Cranial Helmets</li>
                <li><span class="code-tag boc-tag">PD08</span> Lymphedema Garments</li>
                <li><span class="code-tag boc-tag">PD09</span> Ocular Prosthetics</li>
                <li><span class="code-tag boc-tag">PE03</span> Enteral Nutrients</li>
                <li><span class="code-tag boc-tag">PE04</span> Enteral Equipment</li>
                <li><span class="code-tag boc-tag">R07</span> Suction Pumps</li>
                <li><span class="code-tag boc-tag">S01</span> Compression Stockings</li>
                <li><span class="code-tag boc-tag">S04</span> Diabetic Shoes</li>
            </ul>
        </div>
        <div>
            <h4 style="color: #9C27B0;">BOC Quick Check Process</h4>
            <div class="checklist">
                <strong>Before every sale:</strong>
                <ol>
                    <li>Identify product category</li>
                    <li>Match to BOC code</li>
                    <li>Verify you have that BOC licensed</li>
                    <li>If NO match → Cannot sell legally</li>
                    <li>If YES match → Proceed to Layer 2</li>
                </ol>
            </div>
        </div>
    </div>
</div>

<!-- LAYER 2: HCPCS CODES -->
<div class="section" id="layer2">
    <h2>🔢 LAYER 2: HCPCS Product Codes</h2>
    
    <div class="layer-card layer-2">
        <h3>Understanding HCPCS</h3>
        <p><strong>HCPCS (Healthcare Common Procedure Coding System)</strong> is the standardized coding system that identifies 
        exactly what product you're providing. Every DME item has a specific HCPCS code.</p>
        
        <p><strong>Format:</strong> 1 letter + 4 numbers (e.g., E0143, A4253, K0001)</p>
        
        <div class="grid-2">
            <div>
                <h4>HCPCS Code Categories:</h4>
                <ul>
                    <li><strong>A-codes:</strong> Medical/surgical supplies, diabetic supplies</li>
                    <li><strong>E-codes:</strong> Durable medical equipment</li>
                    <li><strong>K-codes:</strong> Temporary codes, wheelchairs</li>
                    <li><strong>L-codes:</strong> Orthotics, prosthetics</li>
                    <li><strong>V-codes:</strong> Vision/hearing</li>
                    <li><strong>B-codes:</strong> Enteral/parenteral</li>
                </ul>
            </div>
            <div>
                <h4>Key HCPCS Principles:</h4>
                <ul>
                    <li>Must be EXACT code - no substitutions</li>
                    <li>CMS updates codes annually (Jan 1)</li>
                    <li>Some codes are LCD/NCD specific</li>
                    <li>Wrong code = claim denial</li>
                    <li>Code must match BOC category</li>
                </ul>
            </div>
        </div>
    </div>

    <h3>HCPCS Code Examples by BOC Category:</h3>
    <table>
        <tr>
            <th>BOC Code</th>
            <th>Common HCPCS Codes</th>
            <th>Product Description</th>
            <th>Important Notes</th>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">DM05</span></td>
            <td>
                <span class="code-tag hcpcs-tag">E0607</span><br>
                <span class="code-tag hcpcs-tag">A4253</span><br>
                <span class="code-tag hcpcs-tag">A4259</span>
            </td>
            <td>
                Blood glucose monitor<br>
                Test strips (50 ct)<br>
                Lancets (100 ct)
            </td>
            <td>Often requires quantity modifiers. Test strips typically allowed 100-300/month based on insulin use.</td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">M05</span></td>
            <td>
                <span class="code-tag hcpcs-tag">E0130</span><br>
                <span class="code-tag hcpcs-tag">E0143</span><br>
                <span class="code-tag hcpcs-tag">E0147</span>
            </td>
            <td>
                Walker, folding<br>
                Walker, folding, wheeled<br>
                Walker with seat
            </td>
            <td>Purchase item (not rental). May require prior auth depending on payer.</td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">M06</span></td>
            <td>
                <span class="code-tag hcpcs-tag">K0001</span><br>
                <span class="code-tag hcpcs-tag">E1130</span><br>
                <span class="code-tag hcpcs-tag">K0005</span>
            </td>
            <td>
                Standard wheelchair<br>
                Lightweight wheelchair<br>
                Ultralightweight wheelchair
            </td>
            <td>Requires face-to-face evaluation. Complex coverage criteria. Many require prior auth.</td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">DM02</span></td>
            <td>
                <span class="code-tag hcpcs-tag">E0163</span><br>
                <span class="code-tag hcpcs-tag">E0165</span><br>
                <span class="code-tag hcpcs-tag">E0168</span>
            </td>
            <td>
                Commode, fixed arms<br>
                Commode, detachable arms<br>
                Commode, bariatric
            </td>
            <td>Purchase item. Must document medical necessity for home use vs hospital bed.</td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">S01</span></td>
            <td>
                <span class="code-tag hcpcs-tag">A6530</span><br>
                <span class="code-tag hcpcs-tag">A6531</span><br>
                <span class="code-tag hcpcs-tag">A6532</span>
            </td>
            <td>
                Below knee, 18-30 mmHg<br>
                Below knee, 30-40 mmHg<br>
                Below knee, 40-50 mmHg
            </td>
            <td>Coverage typically 4 pairs per 6 months. Must document venous insufficiency or related diagnosis.</td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">DM17</span></td>
            <td>
                <span class="code-tag hcpcs-tag">E2402</span><br>
                <span class="code-tag hcpcs-tag">A6550</span>
            </td>
            <td>
                Negative pressure wound therapy pump<br>
                Wound care set for NPWT
            </td>
            <td>Requires detailed wound measurements, photos, physician orders. Recurring supplies monthly.</td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">S04</span></td>
            <td>
                <span class="code-tag hcpcs-tag">A5500</span><br>
                <span class="code-tag hcpcs-tag">A5513</span>
            </td>
            <td>
                Diabetic shoe, molded<br>
                Diabetic insert, custom
            </td>
            <td>Requires physician certification. Limited to 1 pair shoes + 3 pairs inserts per calendar year.</td>
        </tr>
    </table>

    <div class="critical-box">
        <strong>🚨 CRITICAL HCPCS MISTAKES TO AVOID:</strong>
        <ul>
            <li>❌ Using outdated codes from previous years</li>
            <li>❌ Billing "similar" code instead of exact match</li>
            <li>❌ Not verifying HCPCS is covered by payer</li>
            <li>❌ Missing required modifiers for the HCPCS code</li>
            <li>❌ Billing HCPCS code not aligned with your BOC category</li>
        </ul>
    </div>
</div>

<!-- LAYER 3: ICD-10 -->
<div class="section" id="layer3">
    <h2>🏥 LAYER 3: ICD-10 Medical Necessity</h2>
    
    <div class="layer-card layer-3">
        <h3>Why ICD-10 Codes Matter</h3>
        <p><strong>ICD-10 (International Classification of Diseases, 10th Revision)</strong> codes prove medical necessity - 
        the "why" the patient needs the equipment. Without a valid ICD-10 code that logically supports the DME, 
        Medicare will deny the claim as "not medically necessary."</p>
        
        <p><strong>Format:</strong> 3-7 alphanumeric characters, often with a decimal (e.g., E11.9, M25.561, I87.2)</p>
    </div>

    <div class="warning-box">
        <strong>⚠️ MEDICAL NECESSITY RULE:</strong>
        <p>The ICD-10 code(s) must create a logical, medically reasonable connection to the HCPCS equipment. 
        A reasonable person should be able to look at the diagnosis and say "yes, that condition would require this equipment."</p>
        
        <p><strong>Example of GOOD match:</strong><br>
        <span class="code-tag icd-tag">I50.9</span> Heart failure + <span class="code-tag hcpcs-tag">E0143</span> Wheeled walker = ✅ Makes sense</p>
        
        <p><strong>Example of BAD match:</strong><br>
        <span class="code-tag icd-tag">J06.9</span> Common cold + <span class="code-tag hcpcs-tag">E1130</span> Wheelchair = ❌ No logical connection</p>
    </div>

    <h3>Common ICD-10 Codes by DME Category:</h3>
    <table>
        <tr>
            <th>DME Type</th>
            <th>Primary ICD-10 Codes</th>
            <th>Secondary Supporting Codes</th>
            <th>Documentation Tips</th>
        </tr>
        <tr>
            <td><strong>Walkers & Canes</strong></td>
            <td>
                <span class="code-tag icd-tag">R26.81</span> Unsteadiness on feet<br>
                <span class="code-tag icd-tag">M25.561</span> Pain in knee<br>
                <span class="code-tag icd-tag">M16.0</span> Hip osteoarthritis
            </td>
            <td>
                <span class="code-tag icd-tag">Z96.64</span> Joint replacement<br>
                <span class="code-tag icd-tag">M62.81</span> Muscle weakness<br>
                <span class="code-tag icd-tag">G81.94</span> Hemiplegia
            </td>
            <td>Document fall risk assessment, gait evaluation, physical therapy notes</td>
        </tr>
        <tr>
            <td><strong>Wheelchairs</strong></td>
            <td>
                <span class="code-tag icd-tag">G82.50</span> Quadriplegia<br>
                <span class="code-tag icd-tag">I69.351</span> Hemiplegia post-stroke<br>
                <span class="code-tag icd-tag">M41.9</span> Severe scoliosis
            </td>
            <td>
                <span class="code-tag icd-tag">I50.9</span> Heart failure<br>
                <span class="code-tag icd-tag">M79.673</span> Foot/ankle pain<br>
                <span class="code-tag icd-tag">G80.9</span> Cerebral palsy
            </td>
            <td>MUST have face-to-face evaluation within 90 days. Document why they cannot use walker/cane</td>
        </tr>
        <tr>
            <td><strong>Diabetic Supplies</strong></td>
            <td>
                <span class="code-tag icd-tag">E10.9</span> Type 1 diabetes<br>
                <span class="code-tag icd-tag">E11.9</span> Type 2 diabetes<br>
                <span class="code-tag icd-tag">E11.65</span> Type 2 with hyperglycemia
            </td>
            <td>
                <span class="code-tag icd-tag">E11.21</span> Diabetic nephropathy<br>
                <span class="code-tag icd-tag">E11.51</span> Diabetic neuropathy<br>
                <span class="code-tag icd-tag">E11.42</span> Diabetic retinopathy
            </td>
            <td>Document insulin use for higher testing frequency. Include A1C results if available</td>
        </tr>
        <tr>
            <td><strong>Compression Stockings</strong></td>
            <td>
                <span class="code-tag icd-tag">I87.2</span> Venous insufficiency<br>
                <span class="code-tag icd-tag">I83.90</span> Varicose veins<br>
                <span class="code-tag icd-tag">I89.0</span> Lymphedema
            </td>
            <td>
                <span class="code-tag icd-tag">I87.0</span> Post-thrombotic syndrome<br>
                <span class="code-tag icd-tag">I83.10</span> Varicose veins with ulcer
            </td>
            <td>Document edema, skin changes, venous ultrasound if available</td>
        </tr>
        <tr>
            <td><strong>Hospital Beds</strong></td>
            <td>
                <span class="code-tag icd-tag">M48.061</span> Spinal stenosis<br>
                <span class="code-tag icd-tag">I50.9</span> Heart failure<br>
                <span class="code-tag icd-tag">M54.5</span> Low back pain
            </td>
            <td>
                <span class="code-tag icd-tag">R06.02</span> Shortness of breath<br>
                <span class="code-tag icd-tag">J44.1</span> COPD<br>
                <span class="code-tag icd-tag">E66.9</span> Obesity
            </td>
            <td>Document why patient needs positioning changes. Cardiac/pulmonary conditions stronger than pain alone</td>
        </tr>
        <tr>
            <td><strong>Commodes</strong></td>
            <td>
                <span class="code-tag icd-tag">R26.81</span> Unsteadiness on feet<br>
                <span class="code-tag icd-tag">M25.561</span> Pain in knee<br>
                <span class="code-tag icd-tag">Z48.89</span> Post-surgical recovery
            </td>
            <td>
                <span class="code-tag icd-tag">I50.9</span> Heart failure<br>
                <span class="code-tag icd-tag">J44.1</span> COPD
            </td>
            <td>Document distance from bedroom to bathroom, patient's functional limitations</td>
        </tr>
        <tr>
            <td><strong>Wound VAC (NPWT)</strong></td>
            <td>
                <span class="code-tag icd-tag">L89.154</span> Pressure ulcer stage 4<br>
                <span class="code-tag icd-tag">E11.622</span> Diabetic foot ulcer<br>
                <span class="code-tag icd-tag">L97.929</span> Venous leg ulcer
            </td>
            <td>
                <span class="code-tag icd-tag">I70.261</span> Atherosclerosis with gangrene<br>
                <span class="code-tag icd-tag">T81.31</span> Surgical wound dehiscence
            </td>
            <td>MUST document wound size, depth, location with photos. Requires frequent MD evaluations</td>
        </tr>
    </table>

    <div class="critical-box">
        <h4>🚨 ICD-10 CRITICAL RULES:</h4>
        <ol>
            <li><strong>Primary diagnosis must support DME:</strong> The main ICD-10 code should be the strongest justification</li>
            <li><strong>Specificity matters:</strong> Use most specific code available (e.g., M25.561 knee pain RIGHT side, not M25.56)</li>
            <li><strong>Multiple diagnoses strengthen claims:</strong> 2-4 supporting ICD-10 codes create stronger medical necessity</li>
            <li><strong>Codes must be current:</strong> ICD-10 updates October 1 annually - verify codes are still valid</li>
            <li><strong>Physician provides the codes:</strong> You cannot diagnose - must come from ordering physician</li>
        </ol>
    </div>
</div>

<!-- LAYER 4: MODIFIERS -->
<div class="section" id="layer4">
    <h2>🔧 LAYER 4: Modifiers - The Critical Add-Ons</h2>
    
    <div class="layer-card layer-4">
        <h3>What Are Modifiers?</h3>
        <p><strong>Modifiers</strong> are 2-character codes added to HCPCS codes that provide additional information about 
        the service or item. They can make the difference between a paid claim and a denied claim.</p>
        
        <p><strong>Format:</strong> 2 characters (letters or numbers) added after HCPCS code</p>
        <p><strong>Example:</strong> E0143-KX (walker with proof of medical necessity modifier)</p>
    </div>

    <h3>Essential DME Modifiers You MUST Know:</h3>
    <table>
        <tr>
            <th>Modifier</th>
            <th>Full Name</th>
            <th>When Required</th>
            <th>Critical Usage Notes</th>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">KX</span></td>
            <td>Requirements Specified Met</td>
            <td>When policy-specific coverage criteria are met (most common modifier)</td>
            <td><strong>CRITICAL:</strong> Used when you have all required documentation. Tells Medicare "we've met all LCD/NCD requirements." Missing KX = automatic denial for many items.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">GA</span></td>
            <td>ABN on File</td>
            <td>When you have patient sign Advance Beneficiary Notice (ABN)</td>
            <td>Use when you expect Medicare to deny but patient wants item anyway. Allows you to bill patient. Must have signed ABN form.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">GY</span></td>
            <td>Statutorily Excluded</td>
            <td>Item is never covered by Medicare by law</td>
            <td>Use for non-covered items. Claim will deny but properly tracks that it's not a coverage issue. Patient is financially responsible.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">GZ</span></td>
            <td>Expected Denial</td>
            <td>Item doesn't meet medical necessity (no ABN signed)</td>
            <td>Use when you expect denial and DIDN'T get ABN. Medicare denies and you cannot bill patient. Avoid this situation!</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">NU</span></td>
            <td>New Equipment</td>
            <td>When providing brand new DME (not used/refurbished)</td>
            <td>Standard for most purchases. Indicates new, never-used equipment. Required for initial purchase claims.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">RR</span></td>
            <td>Rental</td>
            <td>For capped rental items during rental period</td>
            <td>Use for each monthly rental billing. Common for wheelchairs, hospital beds, oxygen. Rental rules vary by equipment type.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">UE</span></td>
            <td>Used Equipment</td>
            <td>When providing refurbished/used DME</td>
            <td>Payment is 75% of new purchase price. Must document equipment is in excellent condition and cleaned/sanitized.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">BP</span></td>
            <td>Beneficiary Elected Purchase</td>
            <td>Patient chooses to purchase instead of rent (capped rental items)</td>
            <td>Patient must be informed of purchase vs rental option in writing. Use from month 1 if they elect purchase immediately.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">BR</span></td>
            <td>Beneficiary Elected Rental</td>
            <td>Patient chooses to rent instead of purchase (capped rental items)</td>
            <td>If no election documented within 30 days, defaults to rental with BR modifier.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">BU</span></td>
            <td>Beneficiary Undecided</td>
            <td>Patient hasn't decided rent vs purchase after 30 days</td>
            <td>Temporary modifier. Must convert to BP or BR. After 30 days becomes BR by default.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">MS</span></td>
            <td>6-Month Maintenance</td>
            <td>For ongoing maintenance/servicing of capped rental equipment after purchase</td>
            <td>After 13 months of rental (or purchase), can bill for reasonable maintenance fees. Limited to 2 times per year.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">LL</span></td>
            <td>Lease/Rental Applied to Purchase</td>
            <td>When rental payments will apply toward purchase price</td>
            <td>After 13 continuous rental months, equipment transfers to patient. Rental payments count toward purchase.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">RT</span></td>
            <td>Right Side</td>
            <td>For bilateral items when providing right side only</td>
            <td>Example: Right knee brace, right compression stocking. Pair with specific laterality in documentation.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">LT</span></td>
            <td>Left Side</td>
            <td>For bilateral items when providing left side only</td>
            <td>Example: Left ankle brace, left compression stocking. Must match ICD-10 laterality.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">KH</span></td>
            <td>Initial Claim</td>
            <td>First month billing for capped rental DME</td>
            <td>Use for month 1 only of rental period. Signals this is initial provision of equipment.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">KI</span></td>
            <td>Second or Third Month Rental</td>
            <td>Months 2-3 of capped rental</td>
            <td>Use for second and third monthly rental billing only. Different payment rate than KH.</td>
        </tr>
        <tr>
            <td><span class="code-tag modifier-tag">KJ</span></td>
            <td>Months 4-15 Rental</td>
            <td>Months 4 through 15 of capped rental</td>
            <td>Use from month 4 onward until month 13 (when purchase transfers). Payment rate typically 50% of month 1.</td>
        </tr>
    </table>

    <div class="info-box">
        <h4>💡 MODIFIER COMBINATION RULES:</h4>
        <p>Multiple modifiers can be used together. Order matters!</p>
        <p><strong>Example 1:</strong> <span class="code-tag hcpcs-tag">E0143</span><span class="code-tag modifier-tag">KX</span><span class="code-tag modifier-tag">NU</span> = Walker, requirements met, new equipment</p>
        <p><strong>Example 2:</strong> <span class="code-tag hcpcs-tag">K0001</span><span class="code-tag modifier-tag">RR</span><span class="code-tag modifier-tag">KH</span><span class="code-tag modifier-tag">KX</span> = Wheelchair, rental, month 1, requirements met</p>
        <p><strong>Example 3:</strong> <span class="code-tag hcpcs-tag">A6531</span><span class="code-tag modifier-tag">RT</span><span class="code-tag modifier-tag">KX</span> = Compression stocking, right leg, requirements met</p>
    </div>

    <div class="critical-box">
        <h4>🚨 MODIFIER MISTAKES THAT KILL CLAIMS:</h4>
        <ul>
            <li>❌ <strong>Missing KX modifier when LCD requires it</strong> - Automatic denial. Always check LCD for KX requirement.</li>
            <li>❌ <strong>Using wrong rental modifier</strong> - KH for month 1, KI for months 2-3, KJ for months 4+. Wrong modifier = wrong payment.</li>
            <li>❌ <strong>GA without actual ABN form</strong> - Medicare audits can require you to produce the signed ABN. No form = overpayment.</li>
            <li>❌ <strong>Using GZ instead of GA</strong> - GZ means NO ABN, cannot bill patient. Big financial loss!</li>
            <li>❌ <strong>Not using RT/LT for bilateral items</strong> - Claim may deny or pay incorrectly.</li>
        </ul>
    </div>
</div>

<!-- LAYER 5: DOCUMENTATION -->
<div class="section" id="layer5">
    <h2>📄 LAYER 5: Documentation Requirements</h2>
    
    <div class="layer-card layer-5">
        <h3>Documentation: The Foundation of Payment</h3>
        <p>Medicare pays based on documentation. The rule is simple: <strong>If it's not documented, it didn't happen.</strong></p>
        <p>Insufficient documentation is the #1 reason for claim denials and audit takebacks.</p>
    </div>

    <h3>Core Documentation Elements Required for ALL DME:</h3>
    
    <div class="grid-2">
        <div class="info-box">
            <h4>1️⃣ Physician's Written Order (PWO)</h4>
            <p><strong>Must Include:</strong></p>
            <ul>
                <li>✅ Patient's full name</li>
                <li>✅ Detailed description of item</li>
                <li>✅ ICD-10 diagnosis code(s)</li>
                <li>✅ Physician's signature (wet or electronic)</li>
                <li>✅ Physician's NPI number</li>
                <li>✅ Date of order</li>
                <li>✅ Estimated length of need (if rental)</li>
                <li>✅ Specific product specifications</li>
            </ul>
            <p class="highlight-red"><strong>CRITICAL:</strong> PWO must be dated BEFORE delivery date</p>
        </div>
        
        <div class="warning-box">
            <h4>2️⃣ Face-to-Face Encounter Documentation</h4>
            <p><strong>Required for:</strong></p>
            <ul>
                <li>All power wheelchairs/scooters</li>
                <li>Custom manual wheelchairs</li>
                <li>Hospital beds (in some jurisdictions)</li>
                <li>Certain orthotic devices</li>
            </ul>
            <p><strong>Must Include:</strong></p>
            <ul>
                <li>✅ Visit within 90 days before PWO</li>
                <li>✅ By physician or allowed provider (NP/PA)</li>
                <li>✅ Documentation of medical need</li>
                <li>✅ Functional assessment</li>
                <li>✅ Why the specific equipment is needed</li>
            </ul>
        </div>
    </div>

    <h3>Equipment-Specific Documentation:</h3>
    
    <div class="info-box" style="background-color: #E3F2FD; padding: 15px; margin-bottom: 15px;">
        <p style="margin: 0;"><strong>💡 Click on any section below to expand and view detailed requirements:</strong></p>
    </div>
    
    <div class="expandable">
        <div class="expandable-header">
            ▶ WHEELCHAIRS (Standard & Power) - Click to expand
        </div>
        <div class="expandable-content">
            <h4>Required Documentation:</h4>
            <ul>
                <li><strong>Face-to-face evaluation</strong> within 90 days by physician</li>
                <li><strong>Mobility limitation documentation:</strong> Cannot walk functional distances, cannot use cane/walker</li>
                <li><strong>Home assessment:</strong> Can wheelchair fit through doorways? Ramps needed?</li>
                <li><strong>Cognitive ability:</strong> Can patient safely operate power wheelchair?</li>
                <li><strong>Trial period results</strong> (for power wheelchairs)</li>
                <li><strong>Physical/Occupational therapy notes</strong> supporting need</li>
                <li><strong>Seating evaluation</strong> (for complex rehab wheelchairs)</li>
            </ul>
            <h4>Key Phrases in Documentation:</h4>
            <p class="highlight-green">"Patient requires wheelchair for mobility in the home"</p>
            <p class="highlight-green">"Patient cannot ambulate functional distances without excessive fatigue"</p>
            <p class="highlight-green">"Patient cannot use walker/cane due to [specific limitation]"</p>
        </div>
    </div>

    <div class="expandable">
        <div class="expandable-header">
            ▶ HOSPITAL BEDS - Click to expand
        </div>
        <div class="expandable-content">
            <h4>Required Documentation:</h4>
            <ul>
                <li><strong>Medical condition requiring positioning:</strong> Cardiac/pulmonary disease, spinal conditions, post-surgery</li>
                <li><strong>Physician notes</strong> explaining why patient needs head/foot elevation</li>
                <li><strong>Safety concerns:</strong> Risk of aspiration, GERD, severe edema</li>
                <li><strong>Failed alternatives:</strong> Why regular bed with pillows insufficient</li>
            </ul>
            <h4>Strong vs Weak Justifications:</h4>
            <p class="highlight-green">✅ STRONG: "Patient has CHF requiring head elevation to 45 degrees to prevent pulmonary edema and shortness of breath"</p>
            <p class="highlight-red">❌ WEAK: "Patient has back pain and finds bed more comfortable"</p>
        </div>
    </div>

    <div class="expandable">
        <div class="expandable-header">
            ▶ DIABETIC SUPPLIES (BGM, Test Strips) - Click to expand
        </div>
        <div class="expandable-content">
            <h4>Required Documentation:</h4>
            <ul>
                <li><strong>Diabetes diagnosis</strong> with ICD-10 code (E10.x or E11.x)</li>
                <li><strong>Insulin use documentation</strong> (if requesting >100 strips/month)</li>
                <li><strong>Testing frequency order:</strong> Physician must specify how often to test</li>
                <li><strong>Recent A1C results</strong> (strengthens medical necessity)</li>
            </ul>
            <h4>Quantity Guidelines:</h4>
            <table>
                <tr>
                    <th>Patient Status</th>
                    <th>Max Monthly Strips</th>
                    <th>Documentation Needed</th>
                </tr>
                <tr>
                    <td>Non-insulin treated</td>
                    <td>100 strips</td>
                    <td>Diabetes diagnosis only</td>
                </tr>
                <tr>
                    <td>Insulin treated (1x/day)</td>
                    <td>100 strips</td>
                    <td>Insulin documentation</td>
                </tr>
                <tr>
                    <td>Insulin treated (2x/day)</td>
                    <td>200 strips</td>
                    <td>Insulin documentation + MD order for testing frequency</td>
                </tr>
                <tr>
                    <td>Insulin treated (3+/day)</td>
                    <td>300 strips</td>
                    <td>Intensive insulin regimen documentation</td>
                </tr>
            </table>
        </div>
    </div>

    <div class="expandable">
        <div class="expandable-header">
            ▶ WOUND VAC (NPWT) - Click to expand
        </div>
        <div class="expandable-content">
            <h4>Extensive Documentation Required:</h4>
            <ul>
                <li><strong>Wound assessment:</strong> Location, size (length x width x depth), stage/grade</li>
                <li><strong>Photographs:</strong> Initial wound photos with measuring device visible</li>
                <li><strong>Failed conservative treatment:</strong> Document 30 days of moist wound care failed</li>
                <li><strong>Weekly physician wound evaluations:</strong> Progress notes every 7 days</li>
                <li><strong>Wound measurements trending:</strong> Show improvement or lack thereof</li>
                <li><strong>Infection status:</strong> Document if wound is infected, cultured</li>
                <li><strong>Vascular assessment:</strong> For diabetic foot ulcers - ABIs, pulses documented</li>
            </ul>
            <p class="highlight-red"><strong>HIGH AUDIT RISK:</strong> NPWT is heavily audited. Documentation must be impeccable.</p>
        </div>
    </div>

    <div class="expandable">
        <div class="expandable-header">
            ▶ ORTHOTIC DEVICES - Click to expand
        </div>
        <div class="expandable-content">
            <h4>Required Documentation:</h4>
            <ul>
                <li><strong>Diagnosis requiring immobilization/support</strong></li>
                <li><strong>Custom fabricated vs custom fitted distinction:</strong> OR03 requires fabrication from raw materials; OR04 is pre-fab adjusted</li>
                <li><strong>Measurements/casting notes</strong> (for OR03)</li>
                <li><strong>Fitting notes</strong> (for OR04)</li>
                <li><strong>Trial period results</strong> showing device helps patient function</li>
                <li><strong>Failed conservative measures:</strong> OTC braces tried and failed</li>
            </ul>
        </div>
    </div>

    <h3>Critical Documentation Timeline Rules:</h3>
    <div class="critical-box">
        <table>
            <tr>
                <th>Document Type</th>
                <th>Timing Requirement</th>
                <th>Consequence if Violated</th>
            </tr>
            <tr>
                <td>Physician Written Order (PWO)</td>
                <td>Before delivery OR within 21 days after delivery</td>
                <td>Claim denial - no payment</td>
            </tr>
            <tr>
                <td>Face-to-Face Evaluation</td>
                <td>Within 90 days BEFORE PWO date</td>
                <td>Claim denial - must be within window</td>
            </tr>
            <tr>
                <td>Certificate of Medical Necessity (CMN)</td>
                <td>Before delivery OR when requested by Medicare</td>
                <td>Claim denial or audit recoupment</td>
            </tr>
            <tr>
                <td>Detailed Written Order (DWO)</td>
                <td>Before delivery for itemized prior auth items</td>
                <td>Prior auth denial = cannot bill</td>
            </tr>
            <tr>
                <td>Proof of Delivery (POD)</td>
                <td>Within 30 days of delivery</td>
                <td>Audit recoupment - must prove delivered</td>
            </tr>
            <tr>
                <td>Advance Beneficiary Notice (ABN)</td>
                <td>BEFORE delivering suspected non-covered item</td>
                <td>Cannot bill patient if no ABN obtained</td>
            </tr>
        </table>
    </div>

    <div class="success-box">
        <h4>✅ DOCUMENTATION BEST PRACTICES:</h4>
        <ol>
            <li><strong>Get it in writing FIRST:</strong> Never deliver without written order</li>
            <li><strong>Be specific:</strong> "Walker" is not enough. "E0143 wheeled walker with folding frame" is correct</li>
            <li><strong>Date everything:</strong> Undated documents are worthless in audits</li>
            <li><strong>Original signatures:</strong> Stamped signatures may be rejected</li>
            <li><strong>Keep everything for 7 years:</strong> Medicare audit window is 7 years</li>
            <li><strong>Scan immediately:</strong> Paper degrades, gets lost. Digital backup essential</li>
            <li><strong>Face-to-face within 90 days:</strong> Not 91 days. Count carefully</li>
            <li><strong>Get more than minimum:</strong> Extra documentation protects you in audits</li>
        </ol>
    </div>
</div>

<!-- LAYER 6: LCD/NCD -->
<div class="section" id="layer6">
    <h2>📋 LAYER 6: LCD/NCD Coverage Determinations</h2>
    
    <div class="layer-card layer-6">
        <h3>Understanding LCDs and NCDs</h3>
        <p><strong>LCD (Local Coverage Determination):</strong> Regional Medicare policies set by your MAC (Medicare Administrative Contractor). 
        Coverage rules vary by geographic jurisdiction.</p>
        <p><strong>NCD (National Coverage Determination):</strong> Federal Medicare policies that apply nationwide. 
        NCDs override LCDs when both exist for same item.</p>
    </div>

    <div class="warning-box">
        <strong>⚠️ CRITICAL:</strong> You MUST know which LCD applies to your MAC jurisdiction and follow its rules exactly. 
        Each MAC can have different coverage criteria for the same HCPCS code.
    </div>

    <h3>The 4 Medicare MACs and Their Jurisdictions:</h3>
    <table>
        <tr>
            <th>MAC</th>
            <th>Jurisdiction</th>
            <th>States Covered</th>
            <th>Key Focus Areas</th>
        </tr>
        <tr>
            <td><strong>Jurisdiction A</strong><br>(Noridian)</td>
            <td>Western</td>
            <td>AK, AZ, CA, HI, ID, MT, ND, NV, OR, SD, UT, WA, WY</td>
            <td>Known for strict wheelchair criteria, detailed documentation requirements</td>
        </tr>
        <tr>
            <td><strong>Jurisdiction B</strong><br>(NGS)</td>
            <td>Midwest</td>
            <td>IL, IN, KY, MI, MN, OH, WI</td>
            <td>Strong focus on face-to-face documentation, hospital bed restrictions</td>
        </tr>
        <tr>
            <td><strong>Jurisdiction C</strong><br>(CGS)</td>
            <td>Southeast</td>
            <td>AL, AR, GA, LA, MS, NC, SC, TN, TX, VA, WV</td>
            <td>Detailed oxygen therapy LCDs, diabetic shoe program specifics</td>
        </tr>
        <tr>
            <td><strong>Jurisdiction D</strong><br>(Novitas)</td>
            <td>Northeast</td>
            <td>CT, DE, DC, FL, MA, MD, ME, NH, NJ, NY, PA, RI, VT</td>
            <td>Compression stocking criteria, NPWT documentation requirements</td>
        </tr>
    </table>

    <h3>How to Find and Use LCD/NCDs:</h3>
    <div class="grid-2">
        <div class="info-box">
            <h4>Finding Your LCD:</h4>
            <ol>
                <li>Identify your MAC jurisdiction</li>
                <li>Go to MAC's website or cms.gov</li>
                <li>Search by HCPCS code OR product name</li>
                <li>Download the LCD document (usually PDF)</li>
                <li>Read ENTIRE LCD - especially "Coverage Indications"</li>
            </ol>
            <p><strong>Common LCD Document Names:</strong></p>
            <ul>
                <li>L33642 - Wheelchair Options/Accessories</li>
                <li>L33789 - Power Mobility Devices</li>
                <li>L11459 - Home Blood Glucose Monitors</li>
                <li>L33831 - Hospital Beds</li>
            </ul>
        </div>
        
        <div class="warning-box">
            <h4>What LCDs Specify:</h4>
            <ul>
                <li>✅ <strong>Coverage criteria:</strong> Specific conditions for payment</li>
                <li>✅ <strong>Documentation requirements:</strong> What you must have on file</li>
                <li>✅ <strong>ICD-10 codes:</strong> Sometimes lists covered diagnoses</li>
                <li>✅ <strong>Modifiers required:</strong> When to use KX, etc.</li>
                <li>✅ <strong>Frequency limitations:</strong> How often item can be replaced</li>
                <li>✅ <strong>Prior auth requirements:</strong> If pre-approval needed</li>
                <li>✅ <strong>Non-covered scenarios:</strong> When Medicare WON'T pay</li>
            </ul>
        </div>
    </div>

    <h3>Common LCD Requirements by Equipment Type:</h3>
    
    <div class="info-box" style="background-color: #E3F2FD; padding: 15px; margin-bottom: 15px;">
        <p style="margin: 0;"><strong>💡 Click on any LCD section below to expand and view coverage criteria:</strong></p>
    </div>
    
    <div class="expandable">
        <div class="expandable-header">
            ▶ POWER WHEELCHAIRS LCD (L33789) - Click to expand
        </div>
        <div class="expandable-content">
            <h4>Coverage Criteria (Must Meet ALL):</h4>
            <ul>
                <li>✅ Patient has mobility limitation that significantly impairs ADLs</li>
                <li>✅ Patient's mobility limitation cannot be sufficiently resolved by a cane or walker</li>
                <li>✅ Patient doesn't have sufficient upper extremity function to propel manual wheelchair</li>
                <li>✅ Patient can safely operate power wheelchair controls</li>
                <li>✅ Patient has cognitive ability to safely use power wheelchair</li>
                <li>✅ Patient will use wheelchair in the home</li>
                <li>✅ Patient's home can accommodate wheelchair (doorway width, surfaces)</li>
                <li>✅ Face-to-face evaluation within 90 days by physician</li>
                <li>✅ Trial period completed successfully</li>
            </ul>
            <p class="highlight-yellow"><strong>KX modifier REQUIRED when all criteria met</strong></p>
        </div>
    </div>

    <div class="expandable">
        <div class="expandable-header">
            ▶ HOSPITAL BEDS LCD (L33831) - Click to expand
        </div>
        <div class="expandable-content">
            <h4>Coverage Criteria (Must Meet ONE OR MORE):</h4>
            <ul>
                <li>✅ Patient has medical condition requiring positioning (head or foot elevation)</li>
                <li>✅ Patient requires position changes that cannot be accomplished with a regular bed</li>
                <li>✅ Patient requires special features of a hospital bed for medical reasons</li>
            </ul>
            <h4>Documentation Must Include:</h4>
            <ul>
                <li>Specific diagnosis requiring bed positioning</li>
                <li>Why regular bed with pillows is insufficient</li>
                <li>How bed positioning improves medical condition</li>
            </ul>
            <p class="highlight-green"><strong>STRONG diagnoses:</strong> CHF, COPD, GERD with aspiration risk, post-operative positioning</p>
            <p class="highlight-red"><strong>WEAK diagnoses:</strong> Generic back pain, comfort only</p>
        </div>
    </div>

    <div class="expandable">
        <div class="expandable-header">
            ▶ COMPRESSION STOCKINGS LCD - Click to expand
        </div>
        <div class="expandable-content">
            <h4>Coverage Criteria:</h4>
            <ul>
                <li>✅ Patient has diagnosis of venous insufficiency, lymphedema, or related condition</li>
                <li>✅ Patient requires gradient compression 18mmHg or higher</li>
                <li>✅ Patient's condition is stable (not acute DVT)</li>
                <li>✅ Appropriate pressure level prescribed based on severity</li>
            </ul>
            <h4>Frequency Limits:</h4>
            <table>
                <tr>
                    <th>Item</th>
                    <th>Medicare Allowance</th>
                </tr>
                <tr>
                    <td>Knee-high stockings</td>
                    <td>4 pairs per 6 months</td>
                </tr>
                <tr>
                    <td>Thigh-high stockings</td>
                    <td>4 pairs per 6 months</td>
                </tr>
                <tr>
                    <td>Pantyhose</td>
                    <td>4 pairs per 6 months</td>
                </tr>
                <tr>
                    <td>Garter belt/suspenders</td>
                    <td>1 per 6 months</td>
                </tr>
            </table>
        </div>
    </div>

    <div class="critical-box">
        <h4>🚨 LCD COMPLIANCE RULES:</h4>
        <ol>
            <li><strong>Read the ENTIRE LCD:</strong> Don't skim. Every word matters.</li>
            <li><strong>Document every LCD requirement:</strong> If LCD lists 6 criteria, your documentation must address all 6</li>
            <li><strong>Use KX modifier when LCD requires it:</strong> Most LCDs specify KX for "criteria met"</li>
            <li><strong>Don't assume old LCD still applies:</strong> LCDs change. Check quarterly for updates</li>
            <li><strong>NCD overrides LCD:</strong> If both exist, follow NCD</li>
            <li><strong>LCD varies by MAC:</strong> What's covered in Jurisdiction A may not be in Jurisdiction B</li>
        </ol>
    </div>
</div>

<!-- LAYER 7: PRIOR AUTH -->
<div class="section" id="layer7">
    <h2>🔒 LAYER 7: Prior Authorization Requirements</h2>
    
    <div class="layer-card layer-7">
        <h3>What is Prior Authorization?</h3>
        <p><strong>Prior Authorization (PA)</strong> is pre-approval from the payer BEFORE you deliver the equipment. 
        If PA is required and you don't get it, the claim will be denied even with perfect documentation.</p>
    </div>

    <div class="critical-box">
        <strong>🚨 CRITICAL RULE:</strong> Never deliver equipment requiring prior auth until you have written approval in hand. 
        If you deliver first and then PA is denied, you cannot bill Medicare OR the patient = total loss.
    </div>

    <h3>Items That Typically Require Prior Authorization:</h3>
    <table>
        <tr>
            <th>Equipment Category</th>
            <th>PA Required?</th>
            <th>Medicare Program</th>
            <th>Processing Time</th>
        </tr>
        <tr>
            <td><strong>Power Wheelchairs</strong></td>
            <td>✅ YES (most MACs)</td>
            <td>Prior Authorization Program</td>
            <td>10-45 days</td>
        </tr>
        <tr>
            <td><strong>Power Scooters</strong></td>
            <td>✅ YES (most MACs)</td>
            <td>Prior Authorization Program</td>
            <td>10-45 days</td>
        </tr>
        <tr>
            <td><strong>Hospital Beds (standard)</strong></td>
            <td>✅ YES (some states)</td>
            <td>Varies by MAC</td>
            <td>5-10 days</td>
        </tr>
        <tr>
            <td><strong>Seat Lift Mechanisms</strong></td>
            <td>✅ YES</td>
            <td>Prior Authorization Program</td>
            <td>10-30 days</td>
        </tr>
        <tr>
            <td><strong>Support Surfaces (Group 2/3)</strong></td>
            <td>✅ YES</td>
            <td>Prior Authorization Program</td>
            <td>10-30 days</td>
        </tr>
        <tr>
            <td><strong>NPWT (Wound VAC)</strong></td>
            <td>⚠️ SOME states</td>
            <td>Varies by MAC</td>
            <td>5-10 days</td>
        </tr>
        <tr>
            <td><strong>Standard Walkers</strong></td>
            <td>❌ NO</td>
            <td>N/A</td>
            <td>N/A</td>
        </tr>
        <tr>
            <td><strong>Standard Canes</strong></td>
            <td>❌ NO</td>
            <td>N/A</td>
            <td>N/A</td>
        </tr>
        <tr>
            <td><strong>Commodes</strong></td>
            <td>❌ NO (usually)</td>
            <td>N/A</td>
            <td>N/A</td>
        </tr>
        <tr>
            <td><strong>Diabetic Supplies (BGM)</strong></td>
            <td>❌ NO</td>
            <td>N/A</td>
            <td>N/A</td>
        </tr>
        <tr>
            <td><strong>Compression Stockings</strong></td>
            <td>❌ NO (usually)</td>
            <td>N/A</td>
            <td>N/A</td>
        </tr>
    </table>

    <h3>Prior Authorization Process Flow:</h3>
    <div class="workflow-step">
        <h4>Step 1: Determine if PA Required</h4>
        <ul>
            <li>Check MAC website for PA list</li>
            <li>Verify specific HCPCS code requires PA</li>
            <li>Check patient's secondary insurance PA requirements</li>
        </ul>
    </div>
    <div class="arrow-down">⬇</div>
    
    <div class="workflow-step">
        <h4>Step 2: Gather Complete Documentation</h4>
        <ul>
            <li>Detailed Written Order (DWO) from physician</li>
            <li>Face-to-face evaluation notes (if required)</li>
            <li>All supporting medical records</li>
            <li>CMN or standardized forms (if applicable)</li>
            <li>Home assessment (for wheelchairs)</li>
        </ul>
    </div>
    <div class="arrow-down">⬇</div>
    
    <div class="workflow-step">
        <h4>Step 3: Submit PA Request</h4>
        <ul>
            <li>Use MAC's online portal OR fax submission</li>
            <li>Include ALL required documents (incomplete = automatic denial)</li>
            <li>Get confirmation/tracking number</li>
            <li>Note submission date</li>
        </ul>
    </div>
    <div class="arrow-down">⬇</div>
    
    <div class="workflow-step">
        <h4>Step 4: Wait for Decision (DO NOT DELIVER YET)</h4>
        <ul>
            <li>Check status regularly</li>
            <li>Respond immediately to any requests for additional information</li>
            <li>Typical turnaround: 10-45 business days</li>
        </ul>
    </div>
    <div class="arrow-down">⬇</div>
    
    <div class="workflow-step">
        <h4>Step 5: Receive PA Decision</h4>
        <ul>
            <li><strong>APPROVED:</strong> Get PA number. You can now deliver. Include PA number on claim.</li>
            <li><strong>DENIED:</strong> Review denial reason. Fix issues and resubmit OR contact patient about payment options</li>
            <li><strong>PENDING:</strong> Provide additional documentation as requested</li>
        </ul>
    </div>

    <div class="warning-box">
        <h4>⚠️ PRIOR AUTH PITFALLS:</h4>
        <ul>
            <li>❌ <strong>Delivering before PA approved:</strong> Most common error. Financial disaster if denied.</li>
            <li>❌ <strong>PA expiration:</strong> PAs typically valid 60-180 days. Must deliver within that window.</li>
            <li>❌ <strong>Not including PA number on claim:</strong> Claim will deny even with valid PA</li>
            <li>❌ <strong>Incomplete documentation:</strong> Causes immediate denial. Be thorough first time.</li>
            <li>❌ <strong>Changing equipment specs after PA:</strong> If you change model/specifications, PA may be invalidated</li>
        </ul>
    </div>

    <div class="info-box">
        <h4>💡 PRIVATE INSURANCE PRIOR AUTH:</h4>
        <p>Private insurance companies (UHC, Aetna, Cigna, etc.) have their OWN PA requirements separate from Medicare:</p>
        <ul>
            <li>Different portal/process for each payer</li>
            <li>Often require PA for items Medicare doesn't (e.g., walkers, wheelchairs)</li>
            <li>Stricter criteria in many cases</li>
            <li>Must be checked for EVERY non-Medicare patient</li>
            <li>Some require pre-service approval by phone first</li>
        </ul>
        <p class="highlight-yellow"><strong>ALWAYS verify PA requirements with each payer before proceeding</strong></p>
    </div>
</div>

<!-- LAYER 8: CLAIMS DATA -->
<div class="section" id="layer8">
    <h2>📊 LAYER 8: Claims Submission Data Elements</h2>
    
    <div class="layer-card layer-8">
        <h3>The Claims Form: Where Everything Comes Together</h3>
        <p>All the previous layers culminate in the <strong>CMS-1500 claim form</strong> (or electronic equivalent). 
        Every data field must be correct or the claim will reject/deny.</p>
    </div>

    <h3>Essential Data Elements for Every DME Claim:</h3>
    <table>
        <tr>
            <th>Data Element</th>
            <th>Source</th>
            <th>Critical Rules</th>
        </tr>
        <tr>
            <td><strong>Patient Demographics</strong></td>
            <td>Insurance card, patient intake</td>
            <td>Name must match Medicare card exactly. Middle initial included. DOB in correct format.</td>
        </tr>
        <tr>
            <td><strong>Medicare ID Number (MBI)</strong></td>
            <td>Patient's Medicare card</td>
            <td>11 characters. No dashes or spaces. Verify with Medicare eligibility system.</td>
        </tr>
        <tr>
            <td><strong>Ordering Physician NPI</strong></td>
            <td>Physician's written order</td>
            <td>10-digit NPI. Must be the physician who wrote the order. Cannot be facility NPI.</td>
        </tr>
        <tr>
            <td><strong>Supplier NPI</strong></td>
            <td>Your DME business</td>
            <td>Your 10-digit NPI. Must match PECOS registration. Only one NPI per claim.</td>
        </tr>
        <tr>
            <td><strong>Place of Service (POS)</strong></td>
            <td>Delivery location</td>
            <td>
                <span class="code-tag pos-tag">12</span> = Patient's home<br>
                <span class="code-tag pos-tag">31</span> = Skilled nursing facility<br>
                <span class="code-tag pos-tag">32</span> = Assisted living<br>
                <span class="code-tag pos-tag">21</span> = Inpatient hospital (rare for DME)
            </td>
        </tr>
        <tr>
            <td><strong>HCPCS Code + Modifiers</strong></td>
            <td>Product ID + LCD requirements</td>
            <td>Exact code. All required modifiers in correct order. Example: E0143-KX-NU</td>
        </tr>
        <tr>
            <td><strong>ICD-10 Codes</strong></td>
            <td>Physician's order/prescription</td>
            <td>Primary diagnosis first. Up to 12 diagnoses can be listed. All must support medical necessity.</td>
        </tr>
        <tr>
            <td><strong>Date of Service</strong></td>
            <td>Delivery date</td>
            <td>Must be date equipment delivered to patient. Not order date, not billing date.</td>
        </tr>
        <tr>
            <td><strong>Quantity</strong></td>
            <td>What was delivered</td>
            <td>Must match reality. Test strips = number of boxes. Wheelchair = 1. Walker = 1.</td>
        </tr>
        <tr>
            <td><strong>Charge Amount</strong></td>
            <td>Your fee schedule</td>
            <td>Your usual and customary charge. Medicare will adjust to allowable amount.</td>
        </tr>
        <tr>
            <td><strong>Prior Authorization Number</strong></td>
            <td>PA approval letter</td>
            <td>If PA required, must include PA tracking number. Usually 10-15 characters.</td>
        </tr>
        <tr>
            <td><strong>Rendering Provider (if different)</strong></td>
            <td>Individual who delivered/fit equipment</td>
            <td>May be required for complex rehab, orthotics. Must have appropriate credentials.</td>
        </tr>
    </table>

    <h3>Common Claims Submission Errors:</h3>
    <div class="grid-2">
        <div class="critical-box">
            <h4>Errors That Cause Immediate Rejection:</h4>
            <ul>
                <li>❌ Invalid NPI numbers</li>
                <li>❌ Patient not eligible for Medicare on date of service</li>
                <li>❌ Invalid HCPCS code (typo, discontinued code)</li>
                <li>❌ Missing required modifier</li>
                <li>❌ Invalid diagnosis code format</li>
                <li>❌ Supplier not enrolled in PECOS</li>
            </ul>
            <p><strong>Rejection = claim never enters system. Must fix and resubmit.</strong></p>
        </div>
        
        <div class="warning-box">
            <h4>Errors That Cause Denial After Processing:</h4>
            <ul>
                <li>❌ Medical necessity not established</li>
                <li>❌ Frequency limits exceeded</li>
                <li>❌ Diagnosis doesn't support HCPCS code</li>
                <li>❌ Missing documentation (when requested)</li>
                <li>❌ Prior auth required but not obtained</li>
                <li>❌ Item not covered under LCD/NCD</li>
            </ul>
            <p><strong>Denial = claim processed but not paid. Can appeal with additional documentation.</strong></p>
        </div>
    </div>

    <h3>Claim Submission Methods:</h3>
    <div class="grid-3">
        <div class="info-box">
            <h4>Electronic (EDI)</h4>
            <p><strong>Recommended Method</strong></p>
            <ul>
                <li>✅ Fastest (submit today, adjudicate in 14 days)</li>
                <li>✅ Automatic error checking</li>
                <li>✅ Tracking and status updates</li>
                <li>✅ Required for most suppliers</li>
            </ul>
            <p>Use clearinghouse or billing software</p>
        </div>
        
        <div>
            <h4>Paper (CMS-1500)</h4>
            <p><strong>Slow, Error-Prone</strong></p>
            <ul>
                <li>⚠️ 30+ day processing</li>
                <li>⚠️ Higher rejection rate</li>
                <li>⚠️ No tracking</li>
                <li>⚠️ Handwriting issues</li>
            </ul>
            <p>Only use if electronic unavailable</p>
        </div>
        
        <div>
            <h4>Portal Submission</h4>
            <p><strong>MAC-Specific</strong></p>
            <ul>
                <li>Some MACs allow direct portal entry</li>
                <li>Good for single claims</li>
                <li>Immediate validation</li>
                <li>Not scalable for volume</li>
            </ul>
        </div>
    </div>
</div>

<!-- LAYER 9: RENTAL VS PURCHASE -->
<div class="section" id="layer9">
    <h2>💰 LAYER 9: Rental vs Purchase Classifications</h2>
    
    <div class="layer-card layer-9">
        <h3>Understanding DME Payment Categories</h3>
        <p>Not all DME is paid the same way. Medicare has 4 main payment categories that determine how you get paid 
        and how long payment continues.</p>
    </div>

    <h3>The 4 DME Payment Categories:</h3>
    <table>
        <tr>
            <th>Category</th>
            <th>Payment Method</th>
            <th>How It Works</th>
            <th>Common Examples</th>
        </tr>
        <tr>
            <td><strong>Capped Rental (CR)</strong></td>
            <td>Monthly rental payments up to 13 months</td>
            <td>
                • Month 1: 10% of purchase price<br>
                • Months 2-3: 7.5% of purchase price<br>
                • Months 4-13: 7.5% of purchase price<br>
                • After 13 months: Ownership transfers to patient<br>
                • Supplier responsible for maintenance during rental
            </td>
            <td>
                • Power wheelchairs<br>
                • Hospital beds<br>
                • Walkers (some)<br>
                • PAP devices
            </td>
        </tr>
        <tr>
            <td><strong>Inexpensive/Routinely Purchased (IP)</strong></td>
            <td>One-time purchase payment</td>
            <td>
                • Single payment on delivery<br>
                • Patient owns immediately<br>
                • No ongoing supplier responsibility<br>
                • Cannot bill for repairs/maintenance
            </td>
            <td>
                • Standard canes<br>
                • Standard walkers<br>
                • Commodes<br>
                • Crutches
            </td>
        </tr>
        <tr>
            <td><strong>Frequent & Substantial Servicing (FS)</strong></td>
            <td>Monthly rental (no cap)</td>
            <td>
                • Continues monthly as long as medically necessary<br>
                • Supplier maintains ownership<br>
                • Supplier responsible for all maintenance/repairs<br>
                • Must be returned if no longer needed
            </td>
            <td>
                • Oxygen equipment<br>
                • Ventilators<br>
                • Some infusion pumps
            </td>
        </tr>
        <tr>
            <td><strong>Recurring Purchase (OX)</strong></td>
            <td>Purchase every X months</td>
            <td>
                • Purchase payment each time quantity used up<br>
                • Patient owns each batch<br>
                • Frequency limits apply
            </td>
            <td>
                • Diabetic test strips<br>
                • Lancets<br>
                • Urinary catheters<br>
                • Enteral nutrition
            </td>
        </tr>
    </table>

    <h3>Capped Rental Payment Schedule (Most Complex):</h3>
    <div class="info-box">
        <h4>13-Month Capped Rental Lifecycle:</h4>
        <table>
            <tr>
                <th>Month</th>
                <th>Modifier</th>
                <th>Payment Rate</th>
                <th>Actions Required</th>
            </tr>
            <tr>
                <td>1</td>
                <td><span class="code-tag modifier-tag">KH</span></td>
                <td>10% of purchase price</td>
                <td>Deliver equipment. Get signed delivery receipt. Submit claim with KH modifier.</td>
            </tr>
            <tr>
                <td>2</td>
                <td><span class="code-tag modifier-tag">KI</span></td>
                <td>7.5% of purchase price</td>
                <td>Equipment still with patient. Submit monthly claim with KI modifier.</td>
            </tr>
            <tr>
                <td>3</td>
                <td><span class="code-tag modifier-tag">KI</span></td>
                <td>7.5% of purchase price</td>
                <td>Submit monthly claim with KI modifier.</td>
            </tr>
            <tr>
                <td>4-13</td>
                <td><span class="code-tag modifier-tag">KJ</span></td>
                <td>7.5% of purchase price each month</td>
                <td>Submit monthly claims with KJ modifier. Months 4, 5, 6, 7, 8, 9, 10, 11, 12, 13.</td>
            </tr>
            <tr>
                <td>After 13</td>
                <td>-</td>
                <td>No further monthly payments</td>
                <td>Ownership transfers to patient. Supplier can bill for reasonable maintenance/repairs 2x/year with MS modifier.</td>
            </tr>
        </table>
        
        <p class="highlight-yellow"><strong>TOTAL PAID:</strong> 10% + (2 × 7.5%) + (10 × 7.5%) = 10% + 15% + 75% = 100% of purchase price over 13 months</p>
    </div>

    <h3>Purchase Option (BP vs BR Modifiers):</h3>
    <div class="grid-2">
        <div class="info-box">
            <h4>BP - Beneficiary Elected Purchase</h4>
            <ul>
                <li>Patient chooses to PURCHASE instead of rent</li>
                <li>Must be offered in writing at time of delivery</li>
                <li>Payment still spread over 13 months</li>
                <li>Use BP modifier from Month 1</li>
                <li>Ownership transfers after 13 payments</li>
            </ul>
        </div>
        
        <div class="info-box">
            <h4>BR - Beneficiary Elected Rental</h4>
            <ul>
                <li>Patient chooses to RENT</li>
                <li>Default if no choice made within 30 days</li>
                <li>Payment over 13 months</li>
                <li>Use BR modifier from Month 1</li>
                <li>Ownership transfers after 13 payments</li>
            </ul>
        </div>
    </div>

    <div class="warning-box">
        <h4>⚠️ RENTAL RULES YOU MUST FOLLOW:</h4>
        <ol>
            <li><strong>Must offer purchase option:</strong> Patient has right to purchase. Must be in writing with pricing.</li>
            <li><strong>Continuous monthly billing:</strong> Miss a month = restart the rental clock from Month 1</li>
            <li><strong>Returns stop payment:</strong> If patient returns equipment in Month 5, you only get 5 months payment</li>
            <li><strong>Upgrades require new rental:</strong> If patient upgrades to different equipment, new 13-month cycle starts</li>
            <li><strong>Cannot bill after transfer:</strong> After month 13, cannot bill rental. Can only bill maintenance.</li>
        </ol>
    </div>

    <h3>Key Equipment by Payment Category:</h3>
    <div class="grid-2">
        <div>
            <h4>Capped Rental (CR) Items:</h4>
            <ul>
                <li>Power wheelchairs (K0813-K0864)</li>
                <li>Hospital beds (E0250-E0304)</li>
                <li>Patient lifts (E0621-E0642)</li>
                <li>Seat lift mechanisms (E0627-E0629)</li>
                <li>CPAP/BiPAP devices (E0601)</li>
                <li>Some walkers with wheels (E0143)</li>
            </ul>
        </div>
        
        <div>
            <h4>Inexpensive/Purchase (IP) Items:</h4>
            <ul>
                <li>Standard canes (E0100, E0105)</li>
                <li>Standard walkers (E0130)</li>
                <li>Commodes (E0163-E0168)</li>
                <li>Crutches (E0110-E0118)</li>
                <li>Bath/shower chairs (E0240)</li>
                <li>Raised toilet seats (E0244)</li>
            </ul>
        </div>
    </div>
</div>

<!-- LAYER 10: PAYER SPECIFIC -->
<div class="section" id="layer10">
    <h2>🏢 LAYER 10: Payer-Specific Requirements</h2>
    
    <div class="layer-card layer-10">
        <h3>One Size Does NOT Fit All</h3>
        <p>Each payer (Medicare, Medicaid, private insurance) has different rules, different documentation requirements, 
        different coverage policies, and different billing processes. What works for Medicare may not work for Aetna.</p>
    </div>

    <h3>Major Payer Categories and Their Differences:</h3>
    <table>
        <tr>
            <th>Payer Type</th>
            <th>Coverage Scope</th>
            <th>Documentation</th>
            <th>Prior Auth</th>
            <th>Payment Speed</th>
            <th>Special Considerations</th>
        </tr>
        <tr>
            <td><strong>Medicare (Original)</strong></td>
            <td>Follows LCDs/NCDs strictly</td>
            <td>Standardized (PWO, CMN, etc.)</td>
            <td>Required for specific items</td>
            <td>14-30 days (electronic)</td>
            <td>
                • 80/20 split (80% Medicare, 20% patient/secondary)<br>
                • Strict medical necessity<br>
                • 7-year audit window<br>
                • Most predictable rules
            </td>
        </tr>
        <tr>
            <td><strong>Medicare Advantage (MA Plans)</strong></td>
            <td>Can be MORE restrictive than original Medicare</td>
            <td>Often MORE documentation required</td>
            <td>Required for MOST items</td>
            <td>30-45 days</td>
            <td>
                • Each plan has own rules<br>
                • Must be in-network<br>
                • Prior auth almost always needed<br>
                • May deny what original Medicare covers
            </td>
        </tr>
        <tr>
            <td><strong>Medicaid</strong></td>
            <td>Varies by state drastically</td>
            <td>State-specific forms</td>
            <td>Almost always required</td>
            <td>45-90 days (often slower)</td>
            <td>
                • Different rules per state<br>
                • Lower payment rates<br>
                • More restrictions<br>
                • Some states require special Medicaid license
            </td>
        </tr>
        <tr>
            <td><strong>Private Insurance (UHC, Aetna, Cigna, BCBS)</strong></td>
            <td>Wide variation, often narrower than Medicare</td>
            <td>Varies widely</td>
            <td>Usually required</td>
            <td>30-60 days</td>
            <td>
                • Must verify coverage EVERY time<br>
                • Network status matters<br>
                • Each plan is different<br>
                • May have quantity limits stricter than Medicare
            </td>
        </tr>
        <tr>
            <td><strong>Workers' Compensation</strong></td>
            <td>Injury-specific coverage</td>
            <td>Detailed injury documentation</td>
            <td>Always required</td>
            <td>Varies greatly</td>
            <td>
                • Must relate to work injury<br>
                • Case manager approval often needed<br>
                • Can be excellent payment<br>
                • Requires authorization from employer/carrier
            </td>
        </tr>
        <tr>
            <td><strong>VA (Veterans Affairs)</strong></td>
            <td>Veteran-specific</td>
            <td>VA forms and process</td>
            <td>VA approval required</td>
            <td>60+ days</td>
            <td>
                • Must be VA-approved supplier<br>
                • Separate contracting process<br>
                • Good payment rates<br>
                • Complex approval process
            </td>
        </tr>
    </table>

    <h3>Medicare Advantage Plans: Extra Complexity</h3>
    <div class="warning-box">
        <h4>⚠️ MA PLANS ARE NOT THE SAME AS ORIGINAL MEDICARE</h4>
        <p><strong>Common Misconception:</strong> "It's Medicare, so I follow Medicare rules"</p>
        <p><strong>Reality:</strong> MA plans are private insurance that contract with CMS. They can (and do) have MORE restrictive rules than original Medicare.</p>
        
        <h4>Key MA Plan Differences:</h4>
        <ul>
            <li><strong>Prior Auth Required:</strong> Items that don't need PA under original Medicare may require PA under MA</li>
            <li><strong>Network Requirements:</strong> Must be in-network or they won't cover</li>
            <li><strong>Plan-Specific LCDs:</strong> Each MA carrier can have own medical policies</li>
            <li><strong>Different Forms:</strong> May not accept standard Medicare CMN forms</li>
            <li><strong>Stricter Denials:</strong> MA plans deny more frequently than original Medicare</li>
        </ul>
        
        <p class="highlight-red"><strong>ALWAYS call the MA plan before providing equipment to verify coverage and requirements</strong></p>
    </div>

    <h3>State Medicaid Variations (Examples):</h3>
    <div class="grid-2">
        <div class="info-box">
            <h4>California Medicaid (Medi-Cal)</h4>
            <ul>
                <li>Requires TAR (Treatment Authorization Request) for most DME</li>
                <li>Very restrictive formulary</li>
                <li>Low payment rates (often 50% of Medicare)</li>
                <li>Strict quantity limits</li>
                <li>6-month wait for equipment replacement</li>
            </ul>
        </div>
        
        <div class="info-box">
            <h4>Texas Medicaid</h4>
            <ul>
                <li>Prior authorization through MCO</li>
                <li>Must be enrolled with MCO</li>
                <li>Different MCOs have different processes</li>
                <li>Payment similar to Medicare rates</li>
                <li>Face-to-face required for most DME</li>
            </ul>
        </div>
    </div>

    <h3>Private Insurance Pre-Verification Checklist:</h3>
    <div class="checklist">
        <strong>Before providing equipment to ANY private insurance patient, verify:</strong>
        <ol>
            <li>✅ Patient has active coverage (check eligibility)</li>
            <li>✅ DME benefit is included in patient's plan</li>
            <li>✅ You are in-network for patient's plan</li>
            <li>✅ Prior authorization requirements (yes/no, and process)</li>
            <li>✅ Copay/coinsurance amounts</li>
            <li>✅ Deductible status (met or not met)</li>
            <li>✅ Frequency limitations (e.g., 1 wheelchair every 5 years)</li>
            <li>✅ Medical necessity requirements (documentation needed)</li>
            <li>✅ Quantity limits</li>
            <li>✅ Claim submission address/process</li>
            <li>✅ Get reference number from insurance rep</li>
        </ol>
        <p class="highlight-yellow"><strong>Document EVERYTHING from the verification call including rep name, date, time, reference number</strong></p>
    </div>

    <div class="critical-box">
        <h4>🚨 NEVER ASSUME COVERAGE</h4>
        <p><strong>Fatal Mistake:</strong> "They have Blue Cross, we take Blue Cross, so we're good."</p>
        <p><strong>Reality:</strong> "Blue Cross" is hundreds of different plans. Blue Cross PPO Alabama has completely different rules than Blue Cross HMO New York.</p>
        
        <p><strong>MUST VERIFY EVERY PATIENT:</strong></p>
        <ul>
            <li>Even if same insurance carrier</li>
            <li>Even if same employer group</li>
            <li>Even if you've seen that plan before</li>
            <li>Plans change quarterly</li>
        </ul>
    </div>
</div>

<!-- COMPLETE WORKFLOW -->
<div class="section" id="workflow">
    <h2>🔄 Complete DME Claims Workflow: Start to Payment</h2>
    
    <div class="success-box">
        <h3 style="margin-top: 0;">The Perfect DME Transaction - Step by Step</h3>
        <p>This is the complete workflow that brings together all 10 layers. Follow this every time.</p>
    </div>

    <div class="workflow-step" style="border-left-color: #e91e63;">
        <h4>PHASE 1: PATIENT INQUIRY & INITIAL VERIFICATION</h4>
        <ol>
            <li><strong>Patient contacts you</strong> or physician refers patient</li>
            <li><strong>Collect initial information:</strong>
                <ul>
                    <li>Patient demographics</li>
                    <li>Insurance information (front/back of card)</li>
                    <li>What equipment they need</li>
                    <li>Who is prescribing physician</li>
                </ul>
            </li>
            <li><strong>Verify insurance eligibility:</strong>
                <ul>
                    <li>Call insurance or use online portal</li>
                    <li>Confirm active coverage on date of service</li>
                    <li>Document eligibility check</li>
                </ul>
            </li>
            <li><strong>Verify DME benefit:</strong>
                <ul>
                    <li>Does plan cover DME?</li>
                    <li>What are copay/coinsurance/deductible?</li>
                    <li>Any specific coverage limitations?</li>
                </ul>
            </li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #9c27b0;">
        <h4>PHASE 2: BOC & COVERAGE VERIFICATION</h4>
        <ol>
            <li><strong>Identify exact equipment needed</strong> with specific model/features</li>
            <li><strong>Match equipment to BOC category:</strong>
                <ul>
                    <li>Is this within your 36 licensed BOC codes?</li>
                    <li>If NO → Cannot provide, refer elsewhere</li>
                    <li>If YES → Proceed</li>
                </ul>
            </li>
            <li><strong>Identify correct HCPCS code</strong> for exact product</li>
            <li><strong>Check if payer covers this HCPCS code:</strong>
                <ul>
                    <li>Medicare: Check LCD/NCD</li>
                    <li>Private: Ask during verification call</li>
                </ul>
            </li>
            <li><strong>Check payment rate:</strong>
                <ul>
                    <li>Medicare: Look up in fee schedule</li>
                    <li>Private: Get from insurance</li>
                    <li>Calculate profit margin</li>
                </ul>
            </li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #3f51b5;">
        <h4>PHASE 3: DOCUMENTATION GATHERING</h4>
        <ol>
            <li><strong>Contact ordering physician:</strong>
                <ul>
                    <li>Request written order (prescription)</li>
                    <li>Must include patient name, diagnosis (ICD-10), specific equipment, MD signature, NPI</li>
                    <li>Face-to-face documentation if required</li>
                </ul>
            </li>
            <li><strong>Verify ICD-10 codes logically support equipment:</strong>
                <ul>
                    <li>Does diagnosis make sense for this equipment?</li>
                    <li>If questionable, discuss with physician</li>
                </ul>
            </li>
            <li><strong>Gather all supporting documentation:</strong>
                <ul>
                    <li>Medical records</li>
                    <li>Physician notes</li>
                    <li>PT/OT evaluations</li>
                    <li>Home assessment (if required)</li>
                </ul>
            </li>
            <li><strong>Review LCD/NCD requirements:</strong>
                <ul>
                    <li>Do you have documentation for ALL coverage criteria?</li>
                    <li>Any missing elements?</li>
                    <li>Will KX modifier be required?</li>
                </ul>
            </li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #2196f3;">
        <h4>PHASE 4: PRIOR AUTHORIZATION (IF REQUIRED)</h4>
        <ol>
            <li><strong>Determine if PA required:</strong>
                <ul>
                    <li>Check MAC website (for Medicare)</li>
                    <li>Confirmed during insurance verification (private)</li>
                </ul>
            </li>
            <li><strong>If PA required:</strong>
                <ul>
                    <li>Prepare complete PA packet with all documentation</li>
                    <li>Submit through proper channel (portal, fax, mail)</li>
                    <li>Get confirmation number</li>
                    <li>Track submission</li>
                </ul>
            </li>
            <li><strong>Wait for PA decision:</strong>
                <ul>
                    <li>DO NOT DELIVER until approval received</li>
                    <li>Respond to any requests for additional info</li>
                </ul>
            </li>
            <li><strong>If approved:</strong>
                <ul>
                    <li>Note PA number</li>
                    <li>Check PA validity dates</li>
                    <li>Proceed to delivery</li>
                </ul>
            </li>
            <li><strong>If denied:</strong>
                <ul>
                    <li>Review denial reason</li>
                    <li>Determine if can be fixed and resubmitted</li>
                    <li>OR obtain ABN from patient for private pay</li>
                </ul>
            </li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #00bcd4;">
        <h4>PHASE 5: PATIENT EDUCATION & ABN (IF NEEDED)</h4>
        <ol>
            <li><strong>If any chance of denial, obtain ABN:</strong>
                <ul>
                    <li>Explain why Medicare might not cover</li>
                    <li>Provide estimate of patient cost</li>
                    <li>Patient signs ABN form</li>
                    <li>Keep copy for records</li>
                </ul>
            </li>
            <li><strong>Educate patient on equipment use</strong></li>
            <li><strong>Explain financial responsibility:</strong>
                <ul>
                    <li>Copay/coinsurance/deductible amounts</li>
                    <li>When payment is due</li>
                    <li>Rental vs purchase if applicable</li>
                </ul>
            </li>
            <li><strong>Get patient consent for delivery</strong></li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #009688;">
        <h4>PHASE 6: DELIVERY & PROOF OF DELIVERY</h4>
        <ol>
            <li><strong>Schedule delivery</strong> at mutually convenient time</li>
            <li><strong>Deliver equipment to patient:</strong>
                <ul>
                    <li>Bring proper equipment (correct model, clean, functional)</li>
                    <li>Demonstrate use</li>
                    <li>Answer questions</li>
                    <li>Provide instructions/manual</li>
                </ul>
            </li>
            <li><strong>Obtain signed Proof of Delivery:</strong>
                <ul>
                    <li>Patient signature confirming receipt</li>
                    <li>Date of delivery</li>
                    <li>Detailed description of equipment</li>
                    <li>Patient address where delivered</li>
                    <li>Serial numbers if applicable</li>
                </ul>
            </li>
            <li><strong>Document delivery:</strong>
                <ul>
                    <li>Photos if needed</li>
                    <li>Notes on any issues</li>
                    <li>Patient satisfaction</li>
                </ul>
            </li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #4caf50;">
        <h4>PHASE 7: CLAIMS SUBMISSION</h4>
        <ol>
            <li><strong>Prepare claim with all elements:</strong>
                <ul>
                    <li>Patient demographics</li>
                    <li>Insurance information (MBI for Medicare)</li>
                    <li>Ordering physician NPI</li>
                    <li>Your supplier NPI</li>
                    <li>HCPCS code + all required modifiers</li>
                    <li>ICD-10 codes</li>
                    <li>Date of service (delivery date)</li>
                    <li>Place of service code</li>
                    <li>Quantity</li>
                    <li>Charge amount</li>
                    <li>PA number if applicable</li>
                </ul>
            </li>
            <li><strong>Double-check all data entry</strong></li>
            <li><strong>Submit claim electronically:</strong>
                <ul>
                    <li>Through clearinghouse or billing software</li>
                    <li>Within timely filing limits (usually 365 days)</li>
                </ul>
            </li>
            <li><strong>Get submission confirmation</strong></li>
            <li><strong>Document submission date and tracking number</strong></li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #8bc34a;">
        <h4>PHASE 8: CLAIMS TRACKING & FOLLOW-UP</h4>
        <ol>
            <li><strong>Monitor claim status:</strong>
                <ul>
                    <li>Check after 7 days for acceptance/rejection</li>
                    <li>If rejected: Fix error and resubmit immediately</li>
                    <li>If accepted: Track for payment</li>
                </ul>
            </li>
            <li><strong>Follow up if no response after expected timeline:</strong>
                <ul>
                    <li>Medicare: 14-30 days</li>
                    <li>Private: 30-45 days</li>
                </ul>
            </li>
            <li><strong>If denied after processing:</strong>
                <ul>
                    <li>Review denial reason code</li>
                    <li>Gather additional documentation</li>
                    <li>File appeal if appropriate</li>
                    <li>Timeline for appeals is strict (120 days for Medicare)</li>
                </ul>
            </li>
            <li><strong>If documentation requested:</strong>
                <ul>
                    <li>Respond within deadline (30 days typical)</li>
                    <li>Provide ONLY what's requested</li>
                    <li>Keep copy of what you sent</li>
                </ul>
            </li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #ff9800;">
        <h4>PHASE 9: PAYMENT & POSTING</h4>
        <ol>
            <li><strong>Receive payment:</strong>
                <ul>
                    <li>ERA (Electronic Remittance Advice) or paper EOB</li>
                    <li>Review what was paid vs what was billed</li>
                    <li>Note any adjustments</li>
                </ul>
            </li>
            <li><strong>Post payment to patient account:</strong>
                <ul>
                    <li>Update balance</li>
                    <li>Calculate patient responsibility if any</li>
                </ul>
            </li>
            <li><strong>Bill patient for their portion:</strong>
                <ul>
                    <li>Copay, coinsurance, or deductible</li>
                    <li>Cannot bill until insurance processes</li>
                </ul>
            </li>
            <li><strong>Reconcile accounts</strong></li>
        </ol>
    </div>

    <div class="workflow-step" style="border-left-color: #ff5722;">
        <h4>PHASE 10: ONGOING MANAGEMENT (FOR RENTAL/RECURRING)</h4>
        <ol>
            <li><strong>For capped rental items:</strong>
                <ul>
                    <li>Bill monthly with appropriate modifiers (KH, KI, KJ)</li>
                    <li>Track rental months carefully</li>
                    <li>After 13 months, transfer ownership</li>
                </ul>
            </li>
            <li><strong>For recurring purchase items:</strong>
                <ul>
                    <li>Track usage/quantities</li>
                    <li>Reorder and redeliver when appropriate</li>
                    <li>Stay within frequency limits</li>
                </ul>
            </li>
            <li><strong>For maintenance:</strong>
                <ul>
                    <li>After ownership transfer, can bill maintenance MS modifier</li>
                    <li>Limited to 2x per year</li>
                    <li>Must be reasonable charges</li>
                </ul>
            </li>
            <li><strong>Maintain all records for 7 years minimum</strong></li>
        </ol>
    </div>
</div>

<!-- BOC DETAILS SECTION -->
<div class="section" id="boc-details">
    <h2>📊 Your 36 BOC Codes: Detailed Requirements</h2>
    
    <p>Each of your 36 BOC categories has specific coverage criteria, documentation requirements, and common pitfalls. Here's what you need to know for each.</p>

    <!-- Would continue with detailed breakdown of each BOC code with specific HCPCS codes, ICD-10 matches, LCD requirements, etc. -->
    
    <div class="info-box">
        <p><strong>Note:</strong> Due to the extensive nature of detailed BOC coverage, this section would include comprehensive tables for each BOC code including:</p>
        <ul>
            <li>Common HCPCS codes</li>
            <li>Typical ICD-10 codes</li>
            <li>LCD/NCD references</li>
            <li>Documentation requirements</li>
            <li>Common denial reasons</li>
            <li>Best practices</li>
            <li>Profit margin considerations</li>
        </ul>
        <p>Refer to the uploaded BOC codes file for the specific HCPCS codes and product categories under each BOC.</p>
    </div>
</div>

<!-- COMMON ERRORS -->
<div class="section" id="common-errors">
    <h2>🚫 Common Errors That Kill DME Claims</h2>
    
    <h3>Top 20 Most Common DME Billing Mistakes:</h3>
    
    <table>
        <tr>
            <th>#</th>
            <th>Error</th>
            <th>Why It Happens</th>
            <th>How to Fix/Prevent</th>
        </tr>
        <tr>
            <td>1</td>
            <td><strong>Missing KX modifier</strong></td>
            <td>Didn't read LCD requirements</td>
            <td>Always check LCD for modifier requirements. Add KX when all criteria met.</td>
        </tr>
        <tr>
            <td>2</td>
            <td><strong>Delivering before PA approval</strong></td>
            <td>Patient pressure, impatience</td>
            <td>NEVER deliver PA-required items before approval. Financial disaster if denied.</td>
        </tr>
        <tr>
            <td>3</td>
            <td><strong>No face-to-face documentation</strong></td>
            <td>Assumed wasn't needed</td>
            <td>Know which items require F2F. Verify with physician before delivery.</td>
        </tr>
        <tr>
            <td>4</td>
            <td><strong>ICD-10 doesn't support HCPCS</strong></td>
            <td>Took diagnosis from MD without thinking</td>
            <td>Use medical reasoning. Does diagnosis logically require equipment?</td>
        </tr>
        <tr>
            <td>5</td>
            <td><strong>Wrong rental modifier</strong></td>
            <td>Confused KH/KI/KJ sequence</td>
            <td>KH=month 1, KI=months 2-3, KJ=months 4-13. Use correct modifier for month.</td>
        </tr>
        <tr>
            <td>6</td>
            <td><strong>Outdated HCPCS code</strong></td>
            <td>Using old code books</td>
            <td>Update code books annually (Jan 1). Verify codes on cms.gov.</td>
        </tr>
        <tr>
            <td>7</td>
            <td><strong>No signed proof of delivery</strong></td>
            <td>Forgot to get signature</td>
            <td>ALWAYS get signed POD at delivery. Required for audits.</td>
        </tr>
        <tr>
            <td>8</td>
            <td><strong>Operating outside BOC license</strong></td>
            <td>Didn't verify BOC category</td>
            <td>Check every product against your 36 licensed BOCs before selling.</td>
        </tr>
        <tr>
            <td>9</td>
            <td><strong>Using GA instead of GY (or vice versa)</strong></td>
            <td>Confusion about ABN status</td>
            <td>GA = ABN signed (can bill patient). GY = statutorily excluded. GZ = no ABN (can't bill patient).</td>
        </tr>
        <tr>
            <td>10</td>
            <td><strong>Physician order dated AFTER delivery</strong></td>
            <td>Got order retroactively</td>
            <td>PWO must be dated before OR within 21 days after delivery. Get order first!</td>
        </tr>
        <tr>
            <td>11</td>
            <td><strong>Missing physician NPI</strong></td>
            <td>Forgot to collect</td>
            <td>Get NPI at time of order request. Verify with NPPES.</td>
        </tr>
        <tr>
            <td>12</td>
            <td><strong>Treating MA plan like original Medicare</strong></td>
            <td>Assumed same rules</td>
            <td>MA plans are DIFFERENT. Always call to verify requirements.</td>
        </tr>
        <tr>
            <td>13</td>
            <td><strong>Frequency limit violation</strong></td>
            <td>Didn't check previous claims</td>
            <td>Check claims history. Most equipment has replacement timeframes.</td>
        </tr>
        <tr>
            <td>14</td>
            <td><strong>Wrong place of service code</strong></td>
            <td>Used facility code instead of home</td>
            <td>Use POS 12 for patient home delivery. Verify actual delivery location.</td>
        </tr>
        <tr>
            <td>15</td>
            <td><strong>Billing after rental ownership transfer</strong></td>
            <td>Forgot when 13 months completed</td>
            <td>Track rental periods carefully. After month 13, cannot bill rental.</td>
        </tr>
        <tr>
            <td>16</td>
            <td><strong>Not documenting medical necessity</strong></td>
            <td>Assumed diagnosis was enough</td>
            <td>Get physician notes explaining WHY patient needs equipment.</td>
        </tr>
        <tr>
            <td>17</td>
            <td><strong>Missing required CMN</strong></td>
            <td>Didn't know CMN needed</td>
            <td>Some items require CMN (Certificate of Medical Necessity). Check LCD.</td>
        </tr>
        <tr>
            <td>18</td>
            <td><strong>Billing expired LCD</strong></td>
            <td>Using old coverage policy</td>
            <td>Check for LCD updates quarterly. Subscribe to MAC bulletins.</td>
        </tr>
        <tr>
            <td>19</td>
            <td><strong>No ABN when should have gotten one</strong></td>
            <td>Thought it would be covered</td>
            <td>When uncertain about coverage, get ABN. Protects you financially.</td>
        </tr>
        <tr>
            <td>20</td>
            <td><strong>Not responding to documentation requests timely</strong></td>
            <td>Missed deadline</td>
            <td>Respond to ADRs within 30 days. Set up tracking system.</td>
        </tr>
    </table>
</div>

<!-- SYSTEMS NEEDED -->
<div class="section" id="systems">
    <h2>💻 Data Management Systems You Need</h2>
    
    <div class="info-box">
        <h3>To successfully manage all 10 layers, you need robust systems:</h3>
    </div>

    <h3>Essential Software/Systems for DME Business:</h3>
    
    <div class="grid-2">
        <div class="layer-card">
            <h4>1. DME-Specific Billing Software</h4>
            <p><strong>What it does:</strong></p>
            <ul>
                <li>Manages patient demographics</li>
                <li>Tracks insurance eligibility</li>
                <li>Creates and submits claims electronically</li>
                <li>Tracks claim status</li>
                <li>Posts payments</li>
                <li>Manages denials and appeals</li>
                <li>Tracks rental periods and modifiers</li>
            </ul>
            <p><strong>Popular options:</strong> Brightree, Kareo, AccuMED, Fastrack, HomeCare HomeBase</p>
        </div>
        
        <div class="layer-card">
            <h4>2. Inventory Management System</h4>
            <p><strong>What it does:</strong></p>
            <ul>
                <li>Tracks physical inventory</li>
                <li>Serial number tracking</li>
                <li>Ties to HCPCS codes</li>
                <li>Tracks equipment location (patient vs warehouse)</li>
                <li>Manages reordering</li>
                <li>Cost tracking</li>
            </ul>
            <p><strong>Often integrated with billing software</strong></p>
        </div>
        
        <div class="layer-card">
            <h4>3. Document Management System</h4>
            <p><strong>What it does:</strong></p>
            <ul>
                <li>Stores all documentation electronically</li>
                <li>PWOs, prescriptions, ABNs</li>
                <li>Face-to-face documentation</li>
                <li>PODs (Proof of Delivery)</li>
                <li>CMNs and medical records</li>
                <li>Searchable and audit-ready</li>
            </ul>
            <p><strong>Critical for 7-year retention requirement</strong></p>
        </div>
        
        <div class="layer-card">
            <h4>4. Clearinghouse/EDI Service</h4>
            <p><strong>What it does:</strong></p>
            <ul>
                <li>Submits claims electronically to payers</li>
                <li>Receives ERAs (payment info)</li>
                <li>Provides claim tracking</li>
                <li>Error checking before submission</li>
            </ul>
            <p><strong>Popular options:</strong> Change Healthcare, Availity, Office Ally, Waystar</p>
        </div>
        
        <div class="layer-card">
            <h4>5. Prior Authorization Tracking System</h4>
            <p><strong>What it does:</strong></p>
            <ul>
                <li>Tracks PA submissions</li>
                <li>Monitors approval status</li>
                <li>Alerts for PA expirations</li>
                <li>Links PA to patients/orders</li>
            </ul>
            <p><strong>Often part of billing software</strong></p>
        </div>
        
        <div class="layer-card">
            <h4>6. CRM/Patient Communication</h4>
            <p><strong>What it does:</strong></p>
            <ul>
                <li>Manages patient interactions</li>
                <li>Appointment scheduling</li>
                <li>Automated reminders</li>
                <li>Patient satisfaction tracking</li>
                <li>Referral source management</li>
            </ul>
        </div>
        
        <div class="layer-card">
            <h4>7. Compliance Tracking System</h4>
            <p><strong>What it does:</strong></p>
            <ul>
                <li>BOC license management</li>
                <li>PECOS enrollment status</li>
                <li>Accreditation renewals</li>
                <li>Staff credential tracking</li>
                <li>Training compliance</li>
                <li>Audit preparedness</li>
            </ul>
        </div>
        
        <div class="layer-card">
            <h4>8. Fee Schedule Database</h4>
            <p><strong>What it does:</strong></p>
            <ul>
                <li>Medicare fee schedules by MAC</li>
                <li>Private payer contract rates</li>
                <li>Cost data for profitability</li>
                <li>Updated quarterly</li>
            </ul>
            <p><strong>Critical for pricing decisions</strong></p>
        </div>
    </div>

    <h3>Data Points You Must Track:</h3>
    <div class="checklist">
        <strong>For successful DME operations, maintain databases tracking:</strong>
        <ul>
            <li>✅ <strong>Patient master file:</strong> All patient demographics, insurance info, history</li>
            <li>✅ <strong>Physician directory:</strong> NPIs, specialties, contact info, prescription patterns</li>
            <li>✅ <strong>Payer contracts:</strong> Network status, rates, requirements for each payer</li>
            <li>✅ <strong>BOC-to-HCPCS mapping:</strong> Which products fall under which BOC</li>
            <li>✅ <strong>LCD/NCD library:</strong> Current coverage policies for your MAC</li>
            <li>✅ <strong>Inventory master:</strong> All products with HCPCS codes, costs, quantities</li>
            <li>✅ <strong>Rental tracking:</strong> Which patients have rentals, which month, when transfer occurs</li>
            <li>✅ <strong>Claims aging:</strong> Outstanding claims by age, payer, amount</li>
            <li>✅ <strong>Denial tracking:</strong> Reasons for denials, patterns, resolution status</li>
            <li>✅ <strong>Document repository:</strong> All required documentation by patient, searchable</li>
            <li>✅ <strong>Compliance calendar:</strong> License renewals, accreditation dates, training due dates</li>
            <li>✅ <strong>Financial dashboard:</strong> Revenue by BOC category, payer mix, profitability by product</li>
        </ul>
    </div>
</div>

<!-- FINAL SUMMARY -->
<div class="section" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white;">
    <h2 style="color: white; border-bottom-color: white;">🎓 Final Mastery Checklist</h2>
    
    <div style="background: rgba(255,255,255,0.1); padding: 20px; border-radius: 8px; margin: 20px 0;">
        <h3 style="color: white; margin-top: 0;">You've mastered DME coding when you can answer YES to all of these:</h3>
        
        <div class="grid-2">
            <div>
                <h4 style="color: white;">Layer Comprehension:</h4>
                <ul>
                    <li>☐ I know all 36 of my BOC categories by heart</li>
                    <li>☐ I can identify the correct HCPCS code for any product I sell</li>
                    <li>☐ I understand which ICD-10 codes support which equipment</li>
                    <li>☐ I know when to use KX, GA, GY, RR, NU, and rental modifiers</li>
                    <li>☐ I know which documentation is required for each equipment type</li>
                    <li>☐ I know how to find and read LCDs for my MAC jurisdiction</li>
                    <li>☐ I know which items require prior authorization</li>
                    <li>☐ I understand the complete claims submission process</li>
                    <li>☐ I know capped rental vs purchase vs recurring rules</li>
                    <li>☐ I know how Medicare, MA, and private insurance differ</li>
                </ul>
            </div>
            
            <div>
                <h4 style="color: white;">Operational Excellence:</h4>
                <ul>
                    <li>☐ I verify eligibility before EVERY delivery</li>
                    <li>☐ I never deliver PA-required items before approval</li>
                    <li>☐ I get signed POD at every delivery</li>
                    <li>☐ I obtain ABNs when coverage is uncertain</li>
                    <li>☐ I keep all documentation for 7+ years</li>
                    <li>☐ I track rental periods and use correct monthly modifiers</li>
                    <li>☐ I respond to documentation requests within 30 days</li>
                    <li>☐ I review EOBs and identify denial patterns</li>
                    <li>☐ I calculate profitability before accepting orders</li>
                    <li>☐ I have robust software systems to manage all data</li>
                </ul>
            </div>
        </div>
    </div>

    <div style="background: white; padding: 30px; border-radius: 8px; color: #333; text-align: center;">
        <h3 style="color: #2E7D32; margin-top: 0;">The Ultimate DME Success Formula</h3>
        <p style="font-size: 20px; margin: 20px 0;">
            <span class="code-tag boc-tag" style="font-size: 18px;">Valid BOC</span> 
            <strong style="font-size: 28px; color: #FF9800;">+</strong>
            <span class="code-tag hcpcs-tag" style="font-size: 18px;">Correct HCPCS</span>
            <strong style="font-size: 28px; color: #FF9800;">+</strong>
            <span class="code-tag icd-tag" style="font-size: 18px;">Supporting ICD-10</span>
            <strong style="font-size: 28px; color: #FF9800;">+</strong><br>
            <span class="code-tag modifier-tag" style="font-size: 18px;">Right Modifiers</span>
            <strong style="font-size: 28px; color: #FF9800;">+</strong>
            <span style="background-color: #E3F2FD; color: #1565C0; padding: 8px 15px; border-radius: 5px; font-family: monospace; font-weight: bold; font-size: 16px;">Complete Docs</span>
            <strong style="font-size: 28px; color: #FF9800;">+</strong>
            <span style="background-color: #C8E6C9; color: #2E7D32; padding: 8px 15px; border-radius: 5px; font-family: monospace; font-weight: bold; font-size: 16px;">LCD Compliance</span>
            <strong style="font-size: 28px; color: #FF9800;">+</strong><br>
            <span style="background-color: #FFF9C4; color: #F57F17; padding: 8px 15px; border-radius: 5px; font-family: monospace; font-weight: bold; font-size: 16px;">Prior Auth</span>
            <strong style="font-size: 28px; color: #FF9800;">+</strong>
            <span style="background-color: #FFE0B2; color: #E65100; padding: 8px 15px; border-radius: 5px; font-family: monospace; font-weight: bold; font-size: 16px;">Clean Claim Data</span>
            <strong style="font-size: 28px; color: #FF9800;">+</strong>
            <span style="background-color: #FFCDD2; color: #C62828; padding: 8px 15px; border-radius: 5px; font-family: monospace; font-weight: bold; font-size: 16px;">Rental Rules</span>
            <strong style="font-size: 28px; color: #FF9800;">+</strong>
            <span style="background-color: #E1BEE7; color: #6A1B9A; padding: 8px 15px; border-radius: 5px; font-family: monospace; font-weight: bold; font-size: 16px;">Payer Requirements</span>
        </p>
        <p style="font-size: 28px; margin: 30px 0 10px 0;">
            <strong style="font-size: 32px; color: #4CAF50;">=</strong>
        </p>
        <p style="font-size: 32px; margin: 10px 0;">
            <span style="background: linear-gradient(135deg, #4CAF50 0%, #81C784 100%); color: white; padding: 15px 30px; border-radius: 10px; font-weight: bold;">
                💰 CONSISTENT PAYMENT SUCCESS 💰
            </span>
        </p>
    </div>
</div>

<div class="section">
    <p style="text-align: center; color: #666; font-style: italic;">
        This comprehensive guide covers the complete hierarchy of DME coding and billing. 
        Print this, reference it daily, and success will follow. 
        Every claim you submit should go through all 10 layers before delivery.
    </p>
    <p style="text-align: center; color: #666;">
        <strong>Remember:</strong> The difference between a successful DME business and a struggling one 
        is mastering these layers and following them consistently for every single transaction.
    </p>
</div>

<script>
// Enhanced expand/collapse functionality for expandable sections
document.addEventListener('DOMContentLoaded', function() {
    // Get all expandable headers
    var headers = document.querySelectorAll('.expandable-header');
    
    headers.forEach(function(header) {
        // Add click event listener
        header.addEventListener('click', function() {
            var content = this.nextElementSibling;
            
            // Check if content is currently hidden
            var isHidden = content.style.display === 'none' || content.style.display === '';
            
            if (isHidden) {
                // Show the content
                content.style.display = 'block';
                // Change arrow from right (▶) to down (▼)
                this.textContent = this.textContent.replace('▶', '▼');
            } else {
                // Hide the content
                content.style.display = 'none';
                // Change arrow from down (▼) to right (▶)
                this.textContent = this.textContent.replace('▼', '▶');
            }
        });
        
        // Initialize all sections as collapsed
        var content = header.nextElementSibling;
        if (content && content.classList.contains('expandable-content')) {
            content.style.display = 'none';
        }
    });
});
</script>

</body>
</html>
