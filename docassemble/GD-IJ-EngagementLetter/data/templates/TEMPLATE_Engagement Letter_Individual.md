[FILE docassemble.GD-IJ-EngagementLetter:firmlogo.png]

_${ Effective.Date }_

Via Electronic Mail to: _${ Matter.Client.Email }_

 ${ Matter.Client.Prefix } ${ Matter.Client.FirstName } ${ Matter.Client.FirstName }
 ${ Matter.Client.Address }

*Re: Letter of Engagement*

Dear ${ Matter.Client.Prefix } ${ Matter.Client.LastName }:  

You, **${ Matter.Client.FirstName } ${ Matter.Client.FirstName }**, are our client. This letter confirms the terms on which we will represent You. If the matter for which we are being engaged involves an entity, a separate Engagement will be required to represent the entity. Our representation of an entity does not mean that we represent any managers, officers, directors, managers, employees, or shareholders in their individual capacities. 
   
**Scope of Services Covered.**   We will receive a flat fee in exchange for full access to our time, advice, and consultation regarding routine day-to-day legal issues and matters that you may encounter. We refer to these as “general counsel services.” These may include business, corporate, employment, and human resources issues, basic contract or document review and advice, problem solving, pre-litigation negotiation and dispute resolution, and the like.  Whether a matter or issue falls outside the scope of this agreement will be handled with common sense, mutual respect, and fairness to both parties.

**Commencement of Representation.**  We agree that the retainer under this Agreement takes effect as of ${ Effective.Date }. 

**Attorneys' Fees.**

## % if fee_structure is 'flat_fee':
  You agree to pay Innocenti Jones a flat fee of $[NBSP]${ Monthly.Flat.Fee }. At least ${ Pctg.Deposit.Fee } percent of the fee must be received before we will render any services associated with this engagement.
## % elif if fee_structure is 'monthly_retainer':
  You agree to pay Innocenti Jones a monthly flat fee of $[NBSP]${ Monthly.Flat.Fee }. Modification of monthly amount.   After the first ${ Initial.Term } months of this engagement, with reasonable notice, we or you may propose to modify this agreement.  We agree to review the amount of actual time expended and the future expectations and discuss whether an adjustment is appropriate. 
## % elif if fee_structure is 'hourly':
  Fees will be billed monthly and invoiced to client.  Invoices are due and payable  upon receipt. At least $[NBSP]${ Fixed.Deposit.Fee } of the fee must be received before we will render any services associated with this engagement.
## % else:
  Fees will be billed monthly and invoiced to client.  Invoices are due and payable  upon receipt.
## % endif 

**Recording time.**
## % if fee_structure is 'flat_fee' or 'monthly_retainer':
  Our goal is to create an open, flexible relationship that allows you the freedom to consult us without being concerned about the expense associated with every call or email or issue you ask us to consider.  For that reason, we do not anticipate tracking the precise amount of time spent on each individual communication or consultation.  However, to facilitate future discussions about the reasonableness of the amounts incurred, we may track the amount of time spent on substantive projects requiring more than an hour of time.

## % elif if fee_structure is 'hourly':
  You agree to pay at our prevailing rates, attached to this Engagement Letter as Schedule A and are incorporated as if fully set forth herein.

The rates on this schedule are subject to change on 30 days’ written notice to Client.  If Client declines to pay increased rates, Attorney will have the right to withdraw as attorney for Client.

The time charged may include the time Attorney spends on telephone calls relating to Client’s matter, including calls with Client, witnesses, opposing counsel or court personnel.  The legal personnel assigned to Client’s matter may confer among themselves about the matter, as required and appropriate.  When they do confer, each person will charge for the time expended, as long as the work done is reasonably necessary and not duplicative.  Likewise, if more than one of the legal personnel attends a meeting, court hearing or other proceeding, each will charge for the time spent.  Attorney will charge for waiting time in court and elsewhere and for travel time, both local and out of town.  Time is charged in minimum units of one-tenth (. 1) of an hour. 	

## % else:
You agree to pay at our prevailing rates, currently $[NBSP]${ Hourly.Overage.Fee } per hour, and subject to change upon 30 days’ written notice to Client.  If Client declines to pay increased rates, Attorney will have the right to withdraw as attorney for Client.
## % endif 

**Billing for services outside the scope of this agreement.**  If you require services on a matter that we determine falls outside of the scope of this Engagement, we will handle such services on mutually-acceptable fee terms and pursuant to a separate fee agreement. These fee terms may be hourly, a contingent fee, a blend of hourly and contingent, or a lump sum, as we both agree is most appropriate for each separate matter. Our current rates are $[NBSP]${ Hourly.Overage.Fee } per hour. Examples of matters that may fall outside of the scope of general counsel matters are complex commercial transactions, litigation, regulatory matters, or personal matters.

**Termination.** At any time, with reasonable written notice, you or we may terminate this agreement.  If that happens, we agree to comply with all applicable ethical requirements to ensure that you are not prejudiced by that termination. 

**Matters outside of our expertise.** For matters outside of our expertise, such as personal injury, worker’s compensation, real estate, etc., we will advise you that an issue or matter is outside our expertise and, in that event, will make every reasonable effort to refer you to experienced and competent outside counsel.  

**Conflicts of Interest.** We will be bound by our ethical obligations and the Texas Lawyers Creed regarding conflicts of interest, which may require us to decline to provide advice, consultation, or representation on certain matters which would otherwise be considered general counsel matters.  As you utilize our services, we will investigate conflicts or potential conflicts on an ongoing basis and will promptly advise you.

**Dispute resolution.** We agree to make a good faith effort to resolve any question, claim, or issue regarding fees or If we are unable to resolve any differences regarding fees or expenses billed or incurred under this agreement, we both agree to submit the issue to the Fee Dispute Committee of San Antonio Bar Association for resolution and to be bound by that Committee’s decision.    

_Thank you very much for selecting us to represent you.  We look forward to working with you in a mutually beneficial relationship._

Sincerely,

Innocenti Jones PLLC

THE INDIVIDUAL AND ENTITY BELOW AGREE TO RETAIN INNOCENTI JONES PLLC ON THE FOREGOING TERMS.

Dated: ${ Effective.Date }

| for **Innocenti Jones PLLC**                     | for **Client** |
|---------------------------------|-------------|
| /s/ ${ Matter.ResponsibleAttorney.Name }  | By: ${ Client_Signor_Signature } |
| Name:  ${ Matter.ResponsibleAttorney.Name } | Name: ${ Client_Signor_Name } |
| ${ Matter.ResponsibleAttorney.Role }      | Its: ${ Signor.Role } |
| _Address:_  110 E Houston St,  Eighth Floor, Box 120,  San Antonio, Texas 78205      | _Address:_  ${ Client_Address } |

Enclosures: ${ Attachments }

<!-- Questions must include this block
content file:
  - TEMPLATE_Engagement Letter_Outside General Counsel.md
  - Texas_Lawyers_Creed.pdf
  - Rate_Sheet.md
-->
