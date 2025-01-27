.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the FileDialog.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_FileDialog:

FileDialog
==========

**Inherits:** :ref:`ConfirmationDialog<class_ConfirmationDialog>` **<** :ref:`AcceptDialog<class_AcceptDialog>` **<** :ref:`WindowDialog<class_WindowDialog>` **<** :ref:`Popup<class_Popup>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

Dialog for selecting files or directories in the filesystem.

Properties
----------

+-----------------------------------------------+-----------------------------------------------------------------------------+
| :ref:`Access<enum_FileDialog_Access>`         | :ref:`access<class_FileDialog_property_access>`                             |
+-----------------------------------------------+-----------------------------------------------------------------------------+
| :ref:`String<class_String>`                   | :ref:`current_dir<class_FileDialog_property_current_dir>`                   |
+-----------------------------------------------+-----------------------------------------------------------------------------+
| :ref:`String<class_String>`                   | :ref:`current_file<class_FileDialog_property_current_file>`                 |
+-----------------------------------------------+-----------------------------------------------------------------------------+
| :ref:`String<class_String>`                   | :ref:`current_path<class_FileDialog_property_current_path>`                 |
+-----------------------------------------------+-----------------------------------------------------------------------------+
| :ref:`PoolStringArray<class_PoolStringArray>` | :ref:`filters<class_FileDialog_property_filters>`                           |
+-----------------------------------------------+-----------------------------------------------------------------------------+
| :ref:`Mode<enum_FileDialog_Mode>`             | :ref:`mode<class_FileDialog_property_mode>`                                 |
+-----------------------------------------------+-----------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                       | :ref:`mode_overrides_title<class_FileDialog_property_mode_overrides_title>` |
+-----------------------------------------------+-----------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                       | :ref:`show_hidden_files<class_FileDialog_property_show_hidden_files>`       |
+-----------------------------------------------+-----------------------------------------------------------------------------+

Methods
-------

+-------------------------------------------+------------------------------------------------------------------------------------------------------+
| void                                      | :ref:`add_filter<class_FileDialog_method_add_filter>` **(** :ref:`String<class_String>` filter **)** |
+-------------------------------------------+------------------------------------------------------------------------------------------------------+
| void                                      | :ref:`clear_filters<class_FileDialog_method_clear_filters>` **(** **)**                              |
+-------------------------------------------+------------------------------------------------------------------------------------------------------+
| void                                      | :ref:`deselect_items<class_FileDialog_method_deselect_items>` **(** **)**                            |
+-------------------------------------------+------------------------------------------------------------------------------------------------------+
| :ref:`LineEdit<class_LineEdit>`           | :ref:`get_line_edit<class_FileDialog_method_get_line_edit>` **(** **)**                              |
+-------------------------------------------+------------------------------------------------------------------------------------------------------+
| :ref:`VBoxContainer<class_VBoxContainer>` | :ref:`get_vbox<class_FileDialog_method_get_vbox>` **(** **)**                                        |
+-------------------------------------------+------------------------------------------------------------------------------------------------------+
| void                                      | :ref:`invalidate<class_FileDialog_method_invalidate>` **(** **)**                                    |
+-------------------------------------------+------------------------------------------------------------------------------------------------------+

Theme Properties
----------------

+-------------------------------+----------------+
| :ref:`Color<class_Color>`     | files_disabled |
+-------------------------------+----------------+
| :ref:`Texture<class_Texture>` | folder         |
+-------------------------------+----------------+
| :ref:`Texture<class_Texture>` | parent_folder  |
+-------------------------------+----------------+
| :ref:`Texture<class_Texture>` | reload         |
+-------------------------------+----------------+
| :ref:`Texture<class_Texture>` | toggle_hidden  |
+-------------------------------+----------------+

Signals
-------

.. _class_FileDialog_signal_dir_selected:

- **dir_selected** **(** :ref:`String<class_String>` dir **)**

Event emitted when the user selects a directory.

.. _class_FileDialog_signal_file_selected:

- **file_selected** **(** :ref:`String<class_String>` path **)**

Event emitted when the user selects a file (double clicks it or presses the OK button).

.. _class_FileDialog_signal_files_selected:

- **files_selected** **(** :ref:`PoolStringArray<class_PoolStringArray>` paths **)**

Event emitted when the user selects multiple files.

Enumerations
------------

.. _enum_FileDialog_Mode:

.. _class_FileDialog_constant_MODE_OPEN_FILE:

.. _class_FileDialog_constant_MODE_OPEN_FILES:

.. _class_FileDialog_constant_MODE_OPEN_DIR:

.. _class_FileDialog_constant_MODE_OPEN_ANY:

.. _class_FileDialog_constant_MODE_SAVE_FILE:

enum **Mode**:

- **MODE_OPEN_FILE** = **0** --- The dialog allows the selection of one, and only one file.

- **MODE_OPEN_FILES** = **1** --- The dialog allows the selection of multiple files.

- **MODE_OPEN_DIR** = **2** --- The dialog functions as a folder selector, disallowing the selection of any file.

- **MODE_OPEN_ANY** = **3** --- The dialog allows the selection of a file or a directory.

- **MODE_SAVE_FILE** = **4** --- The dialog will warn when a file exists.

.. _enum_FileDialog_Access:

.. _class_FileDialog_constant_ACCESS_RESOURCES:

.. _class_FileDialog_constant_ACCESS_USERDATA:

.. _class_FileDialog_constant_ACCESS_FILESYSTEM:

enum **Access**:

- **ACCESS_RESOURCES** = **0** --- The dialog allows the selection of file and directory.

- **ACCESS_USERDATA** = **1** --- The dialog allows access files under :ref:`Resource<class_Resource>` path(res://) .

- **ACCESS_FILESYSTEM** = **2** --- The dialog allows access files in whole file system.

Description
-----------

FileDialog is a preset dialog used to choose files and directories in the filesystem. It supports filter masks.

Property Descriptions
---------------------

.. _class_FileDialog_property_access:

- :ref:`Access<enum_FileDialog_Access>` **access**

+----------+-------------------+
| *Setter* | set_access(value) |
+----------+-------------------+
| *Getter* | get_access()      |
+----------+-------------------+

The file system access scope. See enum ``Access`` constants.

.. _class_FileDialog_property_current_dir:

- :ref:`String<class_String>` **current_dir**

+----------+------------------------+
| *Setter* | set_current_dir(value) |
+----------+------------------------+
| *Getter* | get_current_dir()      |
+----------+------------------------+

The current working directory of the file dialog.

.. _class_FileDialog_property_current_file:

- :ref:`String<class_String>` **current_file**

+----------+-------------------------+
| *Setter* | set_current_file(value) |
+----------+-------------------------+
| *Getter* | get_current_file()      |
+----------+-------------------------+

The currently selected file of the file dialog.

.. _class_FileDialog_property_current_path:

- :ref:`String<class_String>` **current_path**

+----------+-------------------------+
| *Setter* | set_current_path(value) |
+----------+-------------------------+
| *Getter* | get_current_path()      |
+----------+-------------------------+

The currently selected file path of the file dialog.

.. _class_FileDialog_property_filters:

- :ref:`PoolStringArray<class_PoolStringArray>` **filters**

+----------+--------------------+
| *Setter* | set_filters(value) |
+----------+--------------------+
| *Getter* | get_filters()      |
+----------+--------------------+

Set file type filters. This example shows only .png and .gd files ``set_filters(PoolStringArray(["*.png ; PNG Images","*.gd ; GD Script"]))``.

.. _class_FileDialog_property_mode:

- :ref:`Mode<enum_FileDialog_Mode>` **mode**

+----------+-----------------+
| *Setter* | set_mode(value) |
+----------+-----------------+
| *Getter* | get_mode()      |
+----------+-----------------+

Set dialog to open or save mode, changes selection behavior. See enum ``Mode`` constants.

.. _class_FileDialog_property_mode_overrides_title:

- :ref:`bool<class_bool>` **mode_overrides_title**

+----------+---------------------------------+
| *Setter* | set_mode_overrides_title(value) |
+----------+---------------------------------+
| *Getter* | is_mode_overriding_title()      |
+----------+---------------------------------+

If ``true``, changing the ``Mode`` property will set the window title accordingly (e.g. setting mode to ``MODE_OPEN_FILE`` will change the window title to "Open a File").

.. _class_FileDialog_property_show_hidden_files:

- :ref:`bool<class_bool>` **show_hidden_files**

+----------+------------------------------+
| *Setter* | set_show_hidden_files(value) |
+----------+------------------------------+
| *Getter* | is_showing_hidden_files()    |
+----------+------------------------------+

If ``true``, the dialog will show hidden files.

Method Descriptions
-------------------

.. _class_FileDialog_method_add_filter:

- void **add_filter** **(** :ref:`String<class_String>` filter **)**

Add a custom filter. Example: ``add_filter("*.png ; PNG Images")``

.. _class_FileDialog_method_clear_filters:

- void **clear_filters** **(** **)**

Clear all the added filters in the dialog.

.. _class_FileDialog_method_deselect_items:

- void **deselect_items** **(** **)**

Clear currently selected items in the dialog.

.. _class_FileDialog_method_get_line_edit:

- :ref:`LineEdit<class_LineEdit>` **get_line_edit** **(** **)**

Returns the LineEdit for the selected file.

.. _class_FileDialog_method_get_vbox:

- :ref:`VBoxContainer<class_VBoxContainer>` **get_vbox** **(** **)**

Returns the vertical box container of the dialog, custom controls can be added to it.

.. _class_FileDialog_method_invalidate:

- void **invalidate** **(** **)**

Invalidate and update the current dialog content list.

