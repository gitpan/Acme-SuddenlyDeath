# NAME

Acme::SuddenlyDeath - ASCII Art of sudden death (突然の死) generator

# SYNOPSIS

    use Acme::SuddenlyDeath;

    print sudden_death('突然の死')."\n"
    # outputs =>
    #   ＿人人人人人＿
    #   ＞ 突然の死 ＜
    #   ￣^Y^Y^Y^Y^￣
    print sudden_death("突然の\n死")."\n"
    #   ＿人人人人＿
    #   ＞ 突然の ＜
    #   ＞   死   ＜
    #   ￣^Y^Y^Y^￣
    print sudden_death_single('突然の死')."\n"
    # outputs =>
    #   ＿人人人人人＿＞ 突然の死 ＜￣^Y^Y^Y^Y^￣

# DESCRIPTION

Acme::SuddenlyDeath generate the ASCII Art of sudden death from any strings.
If you would like to know about sudden death, please refer to the following web site (Japanese Web Site).
[http://dic.nicovideo.jp/a/%E7%AA%81%E7%84%B6%E3%81%AE%E6%AD%BB](http://dic.nicovideo.jp/a/%E7%AA%81%E7%84%B6%E3%81%AE%E6%AD%BB)

# METHODS

- sudden\_death

    This method needs a string as parameter.
    It returns multiple line ASCII art of 'sudden death' which was generated from string.

- sudden\_death\_single

    This method needs a string as parameter.
    It returns one line ASCII art of 'sudden death' which was generated from string.

- suddenly\_death
- suddenly\_death\_single

    These methods are similar to the sudden\_death and sudden\_death\_single.
    However, this method decodes the parameter using Encode::decode\_utf8 and encodes the output using Encode::encode\_utf8.

# AUTHOR

papix <mail@papix.net>

# DEPENDENCIES

Text::VisualWidth 0.02 or later.

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.