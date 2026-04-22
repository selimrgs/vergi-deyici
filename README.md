import streamlit as st

st.write("vergi ödeyici")


sayi = st.text_input("ne kadar maş alıyorsun:")

if sayi:

    para = int(sayi)

    kdv = para * 18 / 100
    gelirvergisi = para * 10 / 100

    kalan = para - kdv - gelirvergisi

    st.write("kdv :", kdv)
    st.write("gelirvergisi:", gelirvergisi)
    st.write("kalanpara:")
    st.write(kalan)
