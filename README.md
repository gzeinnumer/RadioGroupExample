# RadioGroupExample

```xml
<RadioGroup
    android:id="@+id/rg"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:checkedButton="@id/radio_1"
    android:orientation="horizontal">

    <RadioButton
        android:id="@+id/radio_1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Internet" />

    <RadioButton
        android:id="@+id/radio_2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Local" />
</RadioGroup>
```

```java
binding.rg.setOnCheckedChangeListener(new RadioGroup.OnCheckedChangeListener(){
    public void onCheckedChanged(RadioGroup group, int checkedId) {
        RadioButton rb = findViewById(checkedId);
        Toast.makeText(getApplicationContext(), "You Selected "+rb.getText(), Toast.LENGTH_SHORT).show();
    }
});
```

---

```
Copyright 2022 M. Fadli Zein
```
