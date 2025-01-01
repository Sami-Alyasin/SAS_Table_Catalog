# SAS Table Catalog

## About
The prupose of this tool is to automate the process of documenting the tables used in SAS proc sql code.

We're using regex (regular expression) to identify patterns in the proc sql code which allows us to capture the table names.

The code will capture the table names even if they're commented, this can be easily modified in the code by commenting this line:

`data = re.sub(r'/\*.*?\*/', '', data, flags=re.DOTALL)`

The code is in a Jupyter Notebook for ease of use.

---

## How to run in Jupyter Notebook
1. Save the proc sql code that you want to pass to this function in a text file.
2. Run the first code block which caontains the gettablenames function.
3. Update the path in the second code block to point to your text file. This should generate all the table names used in your code.

---

## License

This project is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html#license-text). You are free to use, modify, and distribute this code under the terms of the GPLv3. See the [LICENSE](LICENSE) file for details.

---

## Contact

- **Project Maintainer**: Sami Alyasin   
    - **Email**: Sami_Alyasin@outlook.com
    - **GitHub**: [github.com/Sami-Alyasin](https://github.com/Sami-Alyasin)

Feel free to reach out with any questions or suggestions. I hope you find this tool helpful!

---