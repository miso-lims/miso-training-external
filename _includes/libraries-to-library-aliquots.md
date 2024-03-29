<a name="libraries-to-library-aliquots" href="#" id="toplink">top</a>

# 6. Propagating libraries to library aliquots

A library cannot be directly loaded into a _lane_ in a _sequencing container_
(flowcell/SMRTcell) in MISO. A library aliquot must be made and then many aliquots
(or just one) can be mixed into a _pool_ for sequencing.

_Sequencing Orders_ are requests for sequencing pools a certain number of times. They are
used to keep track of sequencing progress for project management and book-keeping.

## 6.1 Bulk creating Library Aliquots
Library aliquots can be made in bulk from libraries.

{% if include.detailed == true %}
<img src="pics/flow-library-aliquot.svg"/>
{% else %}
<img srg="pics/plain-flow-library-aliquot.svg"/>
{% endif %}

In this exercise, we will create library aliquots from the libraries we made previously.

1. On the _Libraries_ page, check all {% if include.detailed == true %}five{% else %}six{% endif %}
   of the libraries you created.
1. From the toolbar, select _Make aliquots_. Click _Create_ in the dialog.
    * Note that the _Make aliquots_ option is also available after bulk creating
      or bulk editing libraries.
1. Enter the library aliquot information:
    * _QC Status_: `{{ site.detailed_qc_status_good }}`
    * _Conc._: Enter any number you wish.
    * _Conc. Units_: `ng/µL`
    * _Creation Date_: Select the current date.
    * _Kit_: Select any.
    * _Kit Lot_: Enter today's date, e.g. `2021-06-15`
{% if include.detailed == true %}
    * _Targeted Sequencing_: Select any if there are options available.
{% endif %}
1. Click _Save_.
