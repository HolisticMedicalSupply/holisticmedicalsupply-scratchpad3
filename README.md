<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Complete Coding System: BOC + HCPCS + ICD-10</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            max-width: 1400px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f5f5f5;
        }
        .section {
            background: white;
            padding: 25px;
            margin: 20px 0;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        h1 {
            color: #333;
            border-bottom: 3px solid #2196F3;
            padding-bottom: 10px;
            text-align: center;
        }
        h2 {
            color: #444;
            margin-top: 0;
        }
        .master-diagram {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 30px;
            border-radius: 12px;
            margin: 30px 0;
        }
        .three-column {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 20px;
            margin: 20px 0;
        }
        .column-box {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }
        .column-box h3 {
            margin-top: 0;
            padding-bottom: 10px;
            border-bottom: 2px solid;
        }
        .boc-box {
            border-left: 5px solid #2196F3;
        }
        .boc-box h3 {
            color: #1976D2;
            border-color: #2196F3;
        }
        .hcpcs-box {
            border-left: 5px solid #FF9800;
        }
        .hcpcs-box h3 {
            color: #F57C00;
            border-color: #FF9800;
        }
        .icd-box {
            border-left: 5px solid #9C27B0;
        }
        .icd-box h3 {
            color: #7B1FA2;
            border-color: #9C27B0;
        }
        .example-box {
            background-color: #F5F5F5;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
            border: 2px solid #2196F3;
        }
        .example-box h4 {
            margin-top: 0;
            color: #1976D2;
        }
        .flow-diagram {
            background-color: #FAFAFA;
            padding: 30px;
            border-radius: 8px;
            margin: 20px 0;
        }
        .flow-step {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            margin: 15px 0;
            border-left: 5px solid #4CAF50;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .flow-step h4 {
            margin: 0 0 10px 0;
            color: #2E7D32;
        }
        .arrow-down {
            text-align: center;
            font-size: 36px;
            color: #4CAF50;
            margin: 10px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
        }
        th {
            background-color: #2196F3;
            color: white;
            padding: 12px;
            text-align: left;
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
            font-family: monospace;
            font-weight: bold;
            margin: 2px;
        }
        .boc-tag {
            background-color: #BBDEFB;
            color: #1976D2;
        }
        .hcpcs-tag {
            background-color: #FFE0B2;
            color: #F57C00;
        }
        .icd-tag {
            background-color: #E1BEE7;
            color: #7B1FA2;
        }
        .critical-box {
            background-color: #FCE4EC;
            padding: 20px;
            border-radius: 8px;
            border: 3px solid #F44336;
            margin: 20px 0;
        }
        .success-box {
            background-color: #E8F5E9;
            padding: 20px;
            border-radius: 8px;
            border: 3px solid #4CAF50;
            margin: 20px 0;
        }
        .checklist {
            background-color: #FFF9C4;
            padding: 15px;
            border-radius: 5px;
            margin: 15px 0;
        }
        ul {
            margin: 10px 0;
        }
        li {
            margin: 8px 0;
        }
    </style>
</head>
<body>

<h1>The Complete DME Coding System<br>BOC + HCPCS + ICD-10</h1>

<div class="master-diagram">
    <h2 style="color: white; text-align: center; margin-top: 0;">The Three-Code System You Must Master</h2>
    
    <div class="three-column">
        <div class="column-box">
            <h3 style="color: #2196F3;">1️⃣ BOC Code</h3>
            <p><strong>Business Operation Code</strong></p>
            <p style="color: #666;">License Category</p>
            <hr style="border-color: rgba(255,255,255,0.3);">
            <p><strong>Purpose:</strong> Defines what you're AUTHORIZED to sell</p>
            <p><strong>Who Controls:</strong> Medicare/CMS accreditation</p>
            <p><strong>You Have:</strong> 36 categories</p>
            <p><strong>Example:</strong> <span class="code-tag boc-tag">DM05</span></p>
        </div>
        
        <div class="column-box">
            <h3 style="color: #FF9800;">2️⃣ HCPCS Code</h3>
            <p><strong>Healthcare Common Procedure Coding System</strong></p>
            <p style="color: #666;">Product Identifier</p>
            <hr style="border-color: rgba(255,255,255,0.3);">
            <p><strong>Purpose:</strong> Identifies WHAT product you sold</p>
            <p><strong>Who Controls:</strong> CMS (updates annually)</p>
            <p><strong>Format:</strong> 1 letter + 4 numbers</p>
            <p><strong>Example:</strong> <span class="code-tag hcpcs-tag">A4253</span></p>
        </div>
        
        <div class="column-box">
            <h3 style="color: #9C27B0;">3️⃣ ICD-10 Code</h3>
            <p><strong>International Classification of Diseases</strong></p>
            <p style="color: #666;">Medical Diagnosis</p>
            <hr style="border-color: rgba(255,255,255,0.3);">
            <p><strong>Purpose:</strong> Proves WHY patient needs it</p>
            <p><strong>Who Controls:</strong> Doctor provides this</p>
            <p><strong>Format:</strong> 3-7 characters with decimal</p>
            <p><strong>Example:</strong> <span class="code-tag icd-tag">E11.9</span></p>
        </div>
    </div>

    <div style="background-color: rgba(255,255,255,0.2); padding: 20px; border-radius: 8px; margin-top: 20px;">
        <h3 style="color: white; text-align: center;">How They Work Together:</h3>
        <p style="text-align: center; font-size: 18px; color: white;">
            <span class="code-tag boc-tag">BOC</span> determines if you CAN sell it +
            <span class="code-tag hcpcs-tag">HCPCS</span> tells insurance WHAT you sold +
            <span class="code-tag icd-tag">ICD-10</span> proves patient NEEDS it
            = <strong>💰 INSURANCE PAYS YOU</strong>
        </p>
    </div>
</div>

<div class="section">
    <h2>📊 The Complete System: How All Three Codes Connect</h2>
    
    <div class="flow-diagram">
        <div class="flow-step">
            <h4>STEP 1: Check Your BOC License</h4>
            <p><strong>Question:</strong> Am I authorized to sell this product type?</p>
            <p><strong>Action:</strong> Look at your 36 licensed BOC categories</p>
            <p><strong>Example:</strong> Patient needs glucose test strips → Check if you have <span class="code-tag boc-tag">DM05</span> (Blood Glucose) → ✓ Yes, you have it</p>
        </div>
        
        <div class="arrow-down">↓</div>
        
        <div class="flow-step">
            <h4>STEP 2: Find the HCPCS Code</h4>
            <p><strong>Question:</strong> What is the exact product code?</p>
            <p><strong>Action:</strong> Find HCPCS code within that BOC category</p>
            <p><strong>Example:</strong> Test strips, 50 count → <span class="code-tag hcpcs-tag">A4253</span></p>
        </div>
        
        <div class="arrow-down">↓</div>
        
        <div class="flow-step">
            <h4>STEP 3: Get Doctor's ICD-10 Code</h4>
            <p><strong>Question:</strong> Why does the patient need this?</p>
            <p><strong>Action:</strong> Doctor provides diagnosis code on prescription</p>
            <p><strong>Example:</strong> Type 2 Diabetes → <span class="code-tag icd-tag">E11.9</span></p>
        </div>
        
        <div class="arrow-down">↓</div>
        
        <div class="flow-step">
            <h4>STEP 4: Verify Codes Match Logically</h4>
            <p><strong>Question:</strong> Does the diagnosis make sense with the product?</p>
            <p><strong>Action:</strong> Confirm medical logic</p>
            <p><strong>Example:</strong> Diabetes (<span class="code-tag icd-tag">E11.9</span>) needs glucose test strips (<span class="code-tag hcpcs-tag">A4253</span>) → ✓ Makes sense</p>
        </div>
        
        <div class="arrow-down">↓</div>
        
        <div class="flow-step" style="border-left-color: #4CAF50; background-color: #E8F5E9;">
            <h4>STEP 5: Submit Claim to Insurance</h4>
            <p><strong>What You Submit:</strong></p>
            <ul>
                <li>✓ BOC category: <span class="code-tag boc-tag">DM05</span> (proves you're licensed)</li>
                <li>✓ HCPCS code: <span class="code-tag hcpcs-tag">A4253</span> (identifies product)</li>
                <li>✓ ICD-10 code: <span class="code-tag icd-tag">E11.9</span> (medical necessity)</li>
                <li>✓ Doctor's prescription with signature</li>
            </ul>
            <p><strong>Result:</strong> <span style="background-color: #4CAF50; color: white; padding: 5px 10px; border-radius: 5px; font-weight: bold;">INSURANCE PAYS YOU ✓</span></p>
        </div>
    </div>
</div>

<div class="section">
    <h2>💡 REAL-WORLD EXAMPLES: Complete Code Sets</h2>
    
    <div class="example-box">
        <h4>Example 1: Diabetic Patient Needs Test Strips</h4>
        
        <table>
            <tr>
                <th>Code Type</th>
                <th>Code</th>
                <th>What It Means</th>
                <th>Who Decides</th>
            </tr>
            <tr style="background-color: #E3F2FD;">
                <td><strong>BOC Code</strong></td>
                <td><span class="code-tag boc-tag">DM05</span></td>
                <td>Blood Glucose Monitors & Supplies (Non-Mail)</td>
                <td>Your License</td>
            </tr>
            <tr style="background-color: #FFE0B2;">
                <td><strong>HCPCS Code</strong></td>
                <td><span class="code-tag hcpcs-tag">A4253</span></td>
                <td>Blood glucose test strips, per 50 strips</td>
                <td>You Select</td>
            </tr>
            <tr style="background-color: #F3E5F5;">
                <td><strong>ICD-10 Code</strong></td>
                <td><span class="code-tag icd-tag">E11.9</span></td>
                <td>Type 2 diabetes mellitus without complications</td>
                <td>Doctor Provides</td>
            </tr>
        </table>
        
        <div class="success-box">
            <strong>✓ COMPLETE SET - Ready to Bill:</strong><br>
            You have license (<span class="code-tag boc-tag">DM05</span>) → Product code (<span class="code-tag hcpcs-tag">A4253</span>) → Medical reason (<span class="code-tag icd-tag">E11.9</span>) → All three codes work together logically → Claim APPROVED
        </div>
    </div>

    <div class="example-box">
        <h4>Example 2: Elderly Patient Needs Walker</h4>
        
        <table>
            <tr>
                <th>Code Type</th>
                <th>Code</th>
                <th>What It Means</th>
                <th>Who Decides</th>
            </tr>
            <tr style="background-color: #E3F2FD;">
                <td><strong>BOC Code</strong></td>
                <td><span class="code-tag boc-tag">M05</span></td>
                <td>Walkers</td>
                <td>Your License</td>
            </tr>
            <tr style="background-color: #FFE0B2;">
                <td><strong>HCPCS Code</strong></td>
                <td><span class="code-tag hcpcs-tag">E0143</span></td>
                <td>Walker, folding, wheeled, adjustable height</td>
                <td>You Select</td>
            </tr>
            <tr style="background-color: #F3E5F5;">
                <td><strong>ICD-10 Code</strong></td>
                <td><span class="code-tag icd-tag">M25.561</span></td>
                <td>Pain in right knee</td>
                <td>Doctor Provides</td>
            </tr>
        </table>
        
        <div class="success-box">
            <strong>✓ COMPLETE SET - Ready to Bill:</strong><br>
            You have license (<span class="code-tag boc-tag">M05</span>) → Product code (<span class="code-tag hcpcs-tag">E0143</span>) → Medical reason (<span class="code-tag icd-tag">M25.561</span>) → Knee pain needs walker = logical → Claim APPROVED
        </div>
    </div>

    <div class="example-box">
        <h4>Example 3: Post-Surgery Patient Needs Commode</h4>
        
        <table>
            <tr>
                <th>Code Type</th>
                <th>Code</th>
                <th>What It Means</th>
                <th>Who Decides</th>
            </tr>
            <tr style="background-color: #E3F2FD;">
                <td><strong>BOC Code</strong></td>
                <td><span class="code-tag boc-tag">DM02</span></td>
                <td>Commodes/Urinals/Bedpans</td>
                <td>Your License</td>
            </tr>
            <tr style="background-color: #FFE0B2;">
                <td><strong>HCPCS Code</strong></td>
                <td><span class="code-tag hcpcs-tag">E0165</span></td>
                <td>Commode chair, mobile, with detachable arms</td>
                <td>You Select</td>
            </tr>
            <tr style="background-color: #F3E5F5;">
                <td><strong>ICD-10 Code</strong></td>
                <td><span class="code-tag icd-tag">R26.81</span></td>
                <td>Difficulty in walking</td>
                <td>Doctor Provides</td>
            </tr>
        </table>
        
        <div class="success-box">
            <strong>✓ COMPLETE SET - Ready to Bill:</strong><br>
            You have license (<span class="code-tag boc-tag">DM02</span>) → Product code (<span class="code-tag hcpcs-tag">E0165</span>) → Medical reason (<span class="code-tag icd-tag">R26.81</span>) → Walking difficulty needs bedside commode = logical → Claim APPROVED
        </div>
    </div>

    <div class="example-box">
        <h4>Example 4: Compression Stockings for Venous Issues</h4>
        
        <table>
            <tr>
                <th>Code Type</th>
                <th>Code</th>
                <th>What It Means</th>
                <th>Who Decides</th>
            </tr>
            <tr style="background-color: #E3F2FD;">
                <td><strong>BOC Code</strong></td>
                <td><span class="code-tag boc-tag">S01</span></td>
                <td>Compression Stockings</td>
                <td>Your License</td>
            </tr>
            <tr style="background-color: #FFE0B2;">
                <td><strong>HCPCS Code</strong></td>
                <td><span class="code-tag hcpcs-tag">A6530</span></td>
                <td>Compression stocking, below knee, 18-30 mmHg</td>
                <td>You Select</td>
            </tr>
            <tr style="background-color: #F3E5F5;">
                <td><strong>ICD-10 Code</strong></td>
                <td><span class="code-tag icd-tag">I87.2</span></td>
                <td>Venous insufficiency (chronic)</td>
                <td>Doctor Provides</td>
            </tr>
        </table>
        
        <div class="success-box">
            <strong>✓ COMPLETE SET - Ready to Bill:</strong><br>
            You have license (<span class="code-tag boc-tag">S01</span>) → Product code (<span class="code-tag hcpcs-tag">A6530</span>) → Medical reason (<span class="code-tag icd-tag">I87.2</span>) → Venous insufficiency requires compression = logical → Claim APPROVED
        </div>
    </div>

    <div class="example-box" style="border-color: #F44336; background-color: #FFEBEE;">
        <h4>❌ WRONG Example: Codes Don't Match</h4>
        
        <table>
            <tr>
                <th>Code Type</th>
                <th>Code</th>
                <th>What It Means</th>
            </tr>
            <tr style="background-color: #E3F2FD;">
                <td><strong>BOC Code</strong></td>
                <td><span class="code-tag boc-tag">M05</span></td>
                <td>Walkers ✓</td>
            </tr>
            <tr style="background-color: #FFE0B2;">
                <td><strong>HCPCS Code</strong></td>
                <td><span class="code-tag hcpcs-tag">E0143</span></td>
                <td>Walker ✓</td>
            </tr>
            <tr style="background-color: #FFCDD2;">
                <td><strong>ICD-10 Code</strong></td>
                <td><span class="code-tag icd-tag">H40.9</span></td>
                <td>Glaucoma (eye disease) ❌</td>
            </tr>
        </table>
        
        <div class="critical-box">
            <strong>❌ CLAIM REJECTED:</strong><br>
            Problem: Eye disease (glaucoma) does NOT logically require a walker. Insurance computer flags this as illogical → <strong>Claim DENIED</strong><br><br>
            
            <strong>Correct ICD-10 codes for walker would be:</strong><br>
            • M25.561 (Knee pain)<br>
            • R26.81 (Difficulty walking)<br>
            • M16.0 (Hip arthritis)<br>
            • I50.9 (Heart failure causing weakness)
        </div>
    </div>
</div>

<div class="section">
    <h2>🎯 Your Complete Code Reference: BOC → HCPCS → ICD-10</h2>
    
    <p><strong>Here are your most profitable combinations to start with:</strong></p>

    <table>
        <tr>
            <th>BOC Category</th>
            <th>HCPCS Codes</th>
            <th>Common ICD-10 Codes</th>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">DM05/06</span><br>Blood Glucose</td>
            <td>
                <span class="code-tag hcpcs-tag">E0607</span> Meter<br>
                <span class="code-tag hcpcs-tag">A4253</span> Test strips<br>
                <span class="code-tag hcpcs-tag">A4259</span> Lancets
            </td>
            <td>
                <span class="code-tag icd-tag">E11.9</span> Type 2 diabetes<br>
                <span class="code-tag icd-tag">E10.9</span> Type 1 diabetes<br>
                <span class="code-tag icd-tag">E11.65</span> Type 2 with hyperglycemia
            </td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">M01</span><br>Canes</td>
            <td>
                <span class="code-tag hcpcs-tag">E0100</span> Standard cane<br>
                <span class="code-tag hcpcs-tag">E0105</span> Quad cane
            </td>
            <td>
                <span class="code-tag icd-tag">M25.561</span> Knee pain<br>
                <span class="code-tag icd-tag">R26.81</span> Difficulty walking<br>
                <span class="code-tag icd-tag">M16.9</span> Hip osteoarthritis
            </td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">M05</span><br>Walkers</td>
            <td>
                <span class="code-tag hcpcs-tag">E0130</span> Standard walker<br>
                <span class="code-tag hcpcs-tag">E0143</span> Wheeled walker<br>
                <span class="code-tag hcpcs-tag">E0147</span> Walker with seat
            </td>
            <td>
                <span class="code-tag icd-tag">M25.561</span> Knee pain<br>
                <span class="code-tag icd-tag">R26.81</span> Difficulty walking<br>
                <span class="code-tag icd-tag">M16.0</span> Hip arthritis<br>
                <span class="code-tag icd-tag">I50.9</span> Heart failure
            </td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">DM02</span><br>Commodes</td>
            <td>
                <span class="code-tag hcpcs-tag">E0163</span> Commode, fixed arms<br>
                <span class="code-tag hcpcs-tag">E0165</span> Commode, detach arms<br>
                <span class="code-tag hcpcs-tag">E0168</span> Bariatric commode
            </td>
            <td>
                <span class="code-tag icd-tag">R26.81</span> Difficulty walking<br>
                <span class="code-tag icd-tag">M25.561</span> Knee pain<br>
                <span class="code-tag icd-tag">Z48.89</span> Post-surgical recovery
            </td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">M06</span><br>Wheelchairs</td>
            <td>
                <span class="code-tag hcpcs-tag">K0001</span> Standard wheelchair<br>
                <span class="code-tag hcpcs-tag">E1130</span> Lightweight wheelchair
            </td>
            <td>
                <span class="code-tag icd-tag">M79.673</span> Foot/ankle pain<br>
                <span class="code-tag icd-tag">M16.0</span> Hip arthritis<br>
                <span class="code-tag icd-tag">I50.9</span> Heart failure<br>
                <span class="code-tag icd-tag">G82.50</span> Quadriplegia
            </td>
        </tr>
        <tr>
            <td><span class="code-tag boc-tag">S01</span><br>Compression Stockings</td>
            <td>
                <span class="code-tag hcpcs-tag">A6530</span> Below knee, 18-30mmHg<br>
                <span class="code-tag hcpcs-tag">A6531</span> Below knee, 30-40mmHg
            </td>
            <td>
                <span class="code-tag icd-tag">I87.2</span> Venous insufficiency<br>
                <span class="code-tag icd-tag">I83.90</span> Varicose veins<br>
                <span class="code-tag icd-tag">I89.0</span> Lymphedema
            </td>
        </tr>
    </table>
</div>

<div class="section">
    <h2>✅ Your Pre-Sale Checklist</h2>
    
    <div class="checklist">
        <h3>Before Providing ANY Product to Patient:</h3>
        <ol>
            <li>
                <strong>☐ BOC License Check</strong><br>
                Question: Is this product within one of my 36 licensed BOC categories?<br>
                Where to check: Your BOC license list (DM02, DM05, M01, M05, etc.)
            </li>
            
            <li>
                <strong>☐ HCPCS Code Identification</strong><br>
                Question: What is the exact HCPCS code for this specific product?<br>
                Where to find: HCPCS code book or CMS website
            </li>
            
            <li>
                <strong>☐ Reimbursement Verification</strong><br>
                Question: How much will Medicare pay for this HCPCS code?<br>
                Where to find: Medicare Fee Schedule for your state
            </li>
            
            <li>
                <strong>☐ Profit Calculation</strong><br>
                Question: Is Medicare payment higher than my wholesale cost?<br>
                Formula: Profit = (Medicare payment) - (Wholesale cost) - (Overhead)
            </li>
            
            <li>
                <strong>☐ Doctor's Prescription</strong><br>
                Question: Do I have a valid prescription with ICD-10 code?<br>
                Must include: Patient diagnosis, ICD-10 code, doctor signature, NPI number
            </li>
            
            <li>
                <strong>☐ Medical Logic Check</strong><br>
                Question: Does the ICD-10 diagnosis logically require this HCPCS equipment?<br>
                Test: Would a reasonable person agree this diagnosis needs this equipment?
            </li>
            
            <li>
                <strong>☐ Documentation Complete</strong><br>
                Required documents:<br>
                ✓ Doctor's prescription<br>
                ✓ ICD-10 diagnosis code<br>
                ✓ Medical necessity statement<br>
                ✓ Patient insurance information<br>
                ✓ Delivery receipt with signature
            </li>
        </ol>
    </div>

    <div class="critical-box">
        <strong>⚠️ CRITICAL WARNING:</strong><br><br>
        
        <strong>If ANY of these checks fail, DO NOT provide the product:</strong><br>
        • No BOC license = Illegal operation<br>
        • Wrong HCPCS code = Claim rejection<br>
        • No ICD-10 code = No medical necessity = No payment<br>
        • Codes don't match logically = Claim denial<br>
        • Incomplete documentation = No reimbursement<br><br>
        
        <strong>Result of skipping these checks: You lose money on the sale.</strong>
    </div>
</div>

<div class="section" style="background-color: #E8F5E9;">
    <h2 style="color: #2E7D32;">🎓 MASTER SUMMARY: The Three-Code System</h2>
    
    <table>
        <tr>
            <th>Code Type</th>
            <th>BOC Code</th>
            <th>HCPCS Code</th>
            <th>ICD-10 Code</th>
        </tr>
        <tr>
            <td><strong>What is it?</strong></td>
            <td>License category</td>
            <td>Product identifier</td>
            <td>Medical diagnosis</td>
        </tr>
        <tr>
            <td><strong>Purpose</strong></td>
            <td>Authorizes you to sell product type</td>
            <td>Tells insurance which product</td>
            <td>Proves medical necessity</td>
        </tr>
        <tr>
            <td><strong>Format</strong></td>
            <td>2-4 letters + numbers<br>(DM05, M01)</td>
            <td>1 letter + 4 numbers<br>(E0143, A4253)</td>
            <td>3-7 characters with decimal<br>(E11.9, M25.561)</td>
        </tr>
        <tr>
            <td><strong>Who controls</strong></td>
            <td>Your accreditation (you have 36)</td>
            <td>CMS (standardized nationally)</td>
            <td>Doctor/Physician</td>
        </tr>
        <tr>
            <td><strong>Who chooses</strong></td>
            <td>Already chosen (your license)</td>
            <td>You choose based on product</td>
            <td>Doctor provides on prescription</td>
        </tr>
        <tr>
            <td><strong>Where to find</strong></td>
            <td>Your BOC license document</td>
            <td>HCPCS code book / CMS website</td>
            <td>Doctor's prescription</td>
        </tr>
        <tr>
            <td><strong>Required for billing?</strong></td>
            <td>Yes (must be licensed)</td>
            <td>Yes (must be exact)</td>
            <td>Yes (must match logically)</td>
        </tr>
        <tr>
            <td><strong>What happens if missing?</strong></td>
            <td>Illegal operation, penalties</td>
            <td>Claim rejected immediately</td>
            <td>No payment (no medical necessity)</td>
        </tr>
    </table>

    <div style="background-color: white; padding: 20px; border-radius: 8px; margin-top: 20px; border: 3px solid #4CAF50;">
        <h3 style="margin-top: 0; color: #2E7D32; text-align: center;">The Golden Rule for DME Success</h3>
        <p style="text-align: center; font-size: 20px; margin: 20px 0;">
            <span class="code-tag boc-tag" style="font-size: 16px;">BOC License</span> 
            <strong style="font-size: 24px; color: #FF9800;">+</strong>
            <span class="code-tag hcpcs-tag" style="font-size: 16px;">Correct HCPCS</span>
            <strong style="font-size: 24px; color: #FF9800;">+</strong>
            <span class="code-tag icd-tag" style="font-size: 16px;">Matching ICD-10</span>
            <strong style="font-size: 24px; color: #4CAF50;">=</strong>
            <span style="background-color: #4CAF50; color: white; padding: 10px 20px; border-radius: 8px; font-weight: bold; font-size: 18px;">💰 PAYMENT SUCCESS</span>
        </p>
    </div>
</div>

</body>
</html>
