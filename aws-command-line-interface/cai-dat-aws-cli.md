---
description: Hướng dẫn cài đặt AWS CLI
cover: >-
  https://images.unsplash.com/photo-1511497584788-876760111969?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=3432&q=80
coverY: 0
---

# Cài đặt AWS CLI

{% hint style="info" %}
Với các hệ điều hành Windows, Linux, MacOS, tham khảo tại [tài liệu hướng dẫn của AWS](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)&#x20;
{% endhint %}

{% tabs %}
{% tab title="WSL2" %}
{% hint style="info" %}
Trong trường hợp wsl2 chưa cài pip3, thực hiện cài pip3 với command:
{% endhint %}

```bash
# Cài đặt python3-pip
$ sudo apt install python3-pip
```



Trên giao diện terminal của wsl2, nhập command:

<pre class="language-bash"><code class="lang-bash"><strong># Cài đặt awscli sử dụng pip
</strong><strong>$ pip3 install awscli --upgrade --user</strong></code></pre>



Kiểm tra cài đặt thành công với command:

```bash
# Kiểm tra awscli đã được cài đặt
$ aws --version
aws-cli/1.25.92 Python/3.10.6 Linux/5.15.68.1-microsoft-standard-WSL2 botocore/1.27.91
```

Khi sử dụng option --user, awscli sẽ được cài đặt tại địa chỉ \~/.local/bin nên nếu kết quả kiểm tra trả về không đúng, cần nhập thêm command sau và kiểm tra lại kết quả

<pre class="language-bash"><code class="lang-bash"><strong>$ export PATH=~/.local/bin:$PATH
</strong><strong>
</strong><strong># Kiểm tra awscli đã được cài đặt
</strong>$ aws --version
aws-cli/1.25.92 Python/3.10.6 Linux/5.15.68.1-microsoft-standard-WSL2 botocore/1.27.91

# Kiểm tra vị trí mà awscli được cài đặt
$ which aws
/home/username/.local/bin/aws</code></pre>
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}





